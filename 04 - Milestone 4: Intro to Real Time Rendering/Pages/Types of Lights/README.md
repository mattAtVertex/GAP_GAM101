# Types of Lights

<h3>Point Lights</h3>
<p><img style="float: right; padding: 0 0 20px 20px;" src="https://vertexschool.instructure.com/courses/203/files/12967/preview?verifier=jPTqMNHhQ4Y4Bb1WPBrZuoEZYfoaQVEXEPJ6LwFg" alt="LightTypes - Point.jpg" width="580" height="328" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/12967" data-api-returntype="File"></p>
<p><strong>Point Lights</strong><span>&nbsp;work much like a real world light bulb, emitting light in all directions from the light bulb's tungsten filament. However, for the sake of performance, Point Lights are simplified down emitting light equally in all directions from just a single point in space. Point lights are great for lights that are meant to extend lights in all directions. You can also adjust the length to simulate something like a tube light.</span></p>
<p>&nbsp;</p>
<p><em><strong>Properties of a Point Light:</strong></em></p>
<ul>
<li>Omni Directional</li>
<li>Radial Light</li>
<li>Good for tube lights, lightbulbs, or other central focus lights</li>
</ul>
<p>&nbsp;</p>
<p>&nbsp;</p>
<hr style="clear: both;">
<h3>Spot Lights</h3>
<p><img style="float: right; padding: 0 0 20px 20px;" src="https://vertexschool.instructure.com/courses/203/files/12969/preview?verifier=tKYk6SjIcnZ25DDf9GIlbdiGl1NEG4byfC2FgSAW" alt="LightTypes - Spot.jpg" width="580" height="328" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/12969" data-api-returntype="File"></p>
<p><strong>Spot lights</strong> are concentrated or focused lights. Similar to point lights, they emit from a central point and fan out into a cone shape. These lights have settings that allow you to control the angle and spred of the projected light cone. The cone consists of an inner and outer cone with different spreads, which allows for a soft contrast or falloff between the two cones.</p>
<p>&nbsp;</p>
<p><em><strong>Properties of a Spot Light:</strong></em></p>
<ul>
<li>Single Directional</li>
<li>Cone shape</li>
<li>Good for overhead lights, actual spot lights, or inset lighting</li>
</ul>
<p>&nbsp;</p>
<hr style="clear: both;">
<h3>Directional Lights</h3>
<p><img style="float: right; padding: 0 0 20px 20px;" src="https://vertexschool.instructure.com/courses/203/files/12965/preview?verifier=LfcoWLHe5rMMnhKJV16RsXrk38DjdYRdIq7BGeHl" alt="LightTypes - Directional.jpg" width="580" height="328" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/12965" data-api-returntype="File"></p>
<p><strong>Directional lights</strong> are a type of light designed to project light from a source that is infinitely far away from your scene. Typically named "Light Source" when creating a New Default Level in Unreal, the Directional Light's primary use is to simulate sun light or moon light. This light source does not radiate from a central point within a scene due to it coming from so far away, so it is controlled by the angle or direction the light is being cast from.</p>
<p>When using a Directional light, you will only ever use one of these in your scene.</p>
<p>&nbsp;</p>
<p><em><strong>Properties of a Directional Light:</strong></em></p>
<ul>
<li>Single Directional</li>
<li>Based on a source too far away to show a central point</li>
<li>Good for sun light and moon light</li>
</ul>
<hr style="clear: both;">
<h3>Sky Lights</h3>
<p><img style="float: right; padding: 0 0 20px 20px;" src="https://vertexschool.instructure.com/courses/203/files/12968/preview?verifier=0E0WFOyqSY70Icm4rilyYwHSwNTnFCQ8NVi0pFAO" alt="Skylight.jpg" width="580" height="657" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/12968" data-api-returntype="File"></p>
<p><strong>Sky lights</strong> are a special case light that does not act like the other lights. These lights simulate an HDRI environment. By default, they take information from your sky and create a virtual HDRI lighting scenario for your scene. Alternatively when using the premade cubemap setting, you can plug in an actual HDRI map that the skylight will use. From there, you can also tint the overall color and control the intensity. The skylight provides ambient light that typically controls the color in your shadows.</p>
<p>When using a sky light, you will only ever use one in your scene.</p>
<p><em><strong>Properties of a Sky Light:</strong></em></p>
<ul>
<li>Special Case Light</li>
<li>Simulates HDRI&nbsp;Based on a skybox and it's color variations or a using a premade cubemap (HDRI texture)</li>
<li>Good for fill light from the sky</li>
<li>Controls the light in the shadows</li>
</ul>
<p>&nbsp;</p>