# Baking and UVs Overview

<p><iframe src="https://www.youtube.com/embed/TJfHWDVjwHE?rel=0" width="800" height="450" allowfullscreen="allowfullscreen" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"></iframe></p>
<hr>
<h2>Objective</h2>
<p>In this handout, we’re going to explore the baking process a little more to understand how it is going to help us later in the texturing phase.</p>
<p><img src="https://vertexschool.instructure.com/courses/203/files/12907/preview?verifier=GKmvlC1qK1KiEchFqfugoinwL82Mq0xVf6pfC8rk" alt="image1.png" width="1920" height="1080" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/12907" data-api-returntype="File"></p>
<hr>
<h2>Baked Maps in 3D Art</h2>
<h3>What is Baking?</h3>
<p>Baking is the process of extracting information from the high poly mesh and mapping it to the UV space of the low poly mesh. Through the baking process, we transfer the details from the high poly to the low poly.</p>
<p>The core map resulting from this process is the Normal Map. This very important map is what fakes lighting information to give the illusion that the low poly has more geometry than it actually does.</p>
<p>But the Normal Map is only one of the many maps that gets baked. There are several other maps generated in the process that contribute to the texturing phase.</p>
<p>&nbsp;</p>
<p><img src="https://vertexschool.instructure.com/courses/203/files/12974/preview?verifier=aGpnzwRGqW27VJG9DHAqILCiLV3eO73NK2fE6cN9" alt="image8.png" width="900" height="506" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/12974" data-api-returntype="File"></p>
<p>&nbsp;</p>
<h3>The Baked Maps</h3>
<p><span>During the baking process, several maps are generated. Each one contributes to the texturing process in a different way, but they are all important for successful texturing.</span></p>
<p>&nbsp;</p>
<p><strong>Normal</strong><span> - Map that fakes lighting to show high poly details on the low poly. Responsible for making the low poly look like it has more geometry than it does.&nbsp;</span></p>
<p><span><img src="https://vertexschool.instructure.com/courses/203/files/12906/preview?verifier=h7kPJKFN7qX89kdR6XZOvM6dnqcubsbm074KS164" alt="image6.png" width="640" height="360" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/12906" data-api-returntype="File"></span></p>
<p><span>&nbsp;</span></p>
<p><strong>Curvature</strong><span> - Map that defines the edges and cavities of the mesh. This is useful for generating edge highlights and controlling areas for dirt and dust.</span></p>
<p><span><img src="https://vertexschool.instructure.com/courses/203/files/12896/preview?verifier=v3ds77Og96Tx09CMEjIxE77JS1aSgJ2VN3puUsul" alt="image7.png" width="640" height="360" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/12896" data-api-returntype="File"></span></p>
<p>&nbsp;</p>
<p><strong>Ambient Occlusion</strong><span> - Map that defines the shadowy areas of the mesh. This map is responsible for the shadows you see in the cracks and crevices, as well as contributing to the control of dust and dirt.</span></p>
<p><strong>Position</strong><span> - Map that stores the position in 3D space as a gradient. This map is important for procedurally generating gradients in your texture work.</span></p>
<p><span><img src="https://vertexschool.instructure.com/courses/203/files/12988/preview?verifier=V9lK61gRvSQXcbBt4Qa8xRPV2Q4lutsjD2CCFWfz" alt="image3.png" width="640" height="360" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/12988" data-api-returntype="File"></span></p>
<p>&nbsp;</p>
<p><strong>Thickness Map</strong><span> - Simulates the thickness of the model. This map is useful for things like SubSurface Scattering.</span></p>
<p><span><img src="https://vertexschool.instructure.com/courses/203/files/12895/preview?verifier=M0bkWlMeaeZ7kcGYN7N07bjJrglLtqlgGQt5Qtw0" alt="image2.png" width="640" height="360" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/12895" data-api-returntype="File"></span></p>
<p>&nbsp;</p>
<p><strong>Material ID</strong><span> - Color map that masks different areas meant for different materials. Another very important map that helps organize the physical materials into groups.</span></p>
<p><span><img src="https://vertexschool.instructure.com/courses/203/files/12970/preview?verifier=OFCeFJwo8oZtSH0BSuoMQQRSG1JGVUbxRd5S2juB" alt="image4.png" width="640" height="360" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/12970" data-api-returntype="File"></span></p>
<p>&nbsp;</p>
<h3>THEY ALL WORK TOGETHER</h3>
<p>&nbsp;</p>
<p><img src="https://vertexschool.instructure.com/courses/203/files/12973/preview?verifier=7UIQut4ckeRCJiIpaEhXEbwB0NFsH9S5PEkWs4hP" alt="image5.png" width="640" height="360" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/12973" data-api-returntype="File"></p>
<hr>
<h2>How Does Projection Work When Baking?</h2>
<p><span>To bake texture maps, the geometry from the high poly source mesh is projected (ray traced) onto the low poly mesh. The best way to visualize this is to imagine a camera looking at the high poly and capturing the direction of the surface for every pixel in the normal map. To make sure the projection does not hit the wrong elements, a cage, or projection mesh must be set up to limit the distance of the projection. For each pixel, the angle of the camera is set by the normal direction of the cage.</span></p>
<p><img src="https://vertexschool.instructure.com/courses/203/files/12990/preview?verifier=YTkDYMSDYwfR3EpahglQ8YOhUR2cCdhVJ7AOZNpL" alt="cagedisplay-1.gif" width="900" height="432" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/12990" data-api-returntype="File">&nbsp;&nbsp;</p>