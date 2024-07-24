# Bake Method: Explode Baking

<p><iframe src="https://www.youtube.com/embed/7Ff9V4H-cfU?rel=0" width="960" height="540" allowfullscreen="allowfullscreen" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" data-mce-fragment="1"></iframe></p>
<h3 style="text-align: left;">BAKING SETUP</h3>
<div class="col span_12 dark left" style="text-align: left;">
<div class="vc_col-sm-12 wpb_column column_container vc_column_container col no-extra-padding instance-8" data-t-w-inherits="default" data-border-radius="none" data-shadow="none" data-border-animation="" data-border-animation-delay="" data-border-width="none" data-border-style="solid" data-border-color="" data-bg-cover="" data-padding-pos="all" data-has-bg-color="false" data-bg-color="" data-bg-opacity="1" data-hover-bg="" data-hover-bg-opacity="1" data-animation="" data-delay="0">
<div class="vc_column-inner">
<div class="wpb_wrapper">
<p style="padding-left: 40px;">1.In your modeling package of choice, group all the objects together.</p>
<p style="padding-left: 40px;">2.Low poly objects in one group</p>
<p style="padding-left: 40px;">3.High poly objects in another. (Make sure both groups are in the same world space)</p>
<p style="text-align: left;"><img src="https://vertexschool.instructure.com/courses/203/files/16080/preview?verifier=8X5v1FwCJPvawflvIcUKXupmf2YxmMdRIwWiiCcA" alt="exbake_01.jpg" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/16080" data-api-returntype="File"></p>
<p style="text-align: left;">&nbsp;</p>
<p style="padding-left: 40px;"><span>4.Duplicate both groups.</span></p>
<p style="padding-left: 40px;"><span>5.Hide the original low poly and high poly groups.</span></p>
<p style="padding-left: 40px;"><span>6.Select the high and low corresponding objects and move them away. </span></p>
<p style="padding-left: 40px;"><span>7.Repeat this with all objects until there is a substantial distance between each object. </span></p>
<p style="padding-left: 40px;"><span>(For example: “outer box” high and low will still both occupy the same world space.)</span></p>
<p>&nbsp;</p>
<p><img src="https://vertexschool.instructure.com/courses/203/files/16081/preview?verifier=wk54ZCcgrCxRLkrTlvfPax41mlykjeVE0oAMmZwJ" alt="exbake_02.jpg" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/16081" data-api-returntype="File"></p>
<p>&nbsp;</p>
<p style="padding-left: 40px;"><span>8. Export the “exploded” low group as an fbx.</span></p>
<p style="padding-left: 40px;"><span>9. Repeat with the “exploded” high group. </span></p>
<p style="padding-left: 40px;"><span>10. Export your original low poly group with all the objects in the original world space as an fbx as well.</span></p>
<p style="padding-left: 40px;"><span>11. Inside of Substance Painter start a new project using the “exploded” low poly fbx</span></p>
<p>&nbsp;</p>
<p><img src="https://vertexschool.instructure.com/courses/203/files/16082/preview?verifier=I4yRN6G4VxeB7GAYFi5OHo2IgfJmMARM7DOc8Gd8" alt="exbake_03.jpg" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/16082" data-api-returntype="File"></p>
<p>&nbsp;</p>
<p style="padding-left: 40px;"><span>12. Bake the mesh maps using the “exploded” high poly fbx. </span></p>
<p style="padding-left: 40px;"><span>13. Once the bake is complete, navigate to the Edit menu. </span></p>
<p style="padding-left: 40px;"><span>14. Select the Project Configuration menu.</span></p>
<p style="text-align: left;">&nbsp;</p>
<p style="text-align: left;"><img src="https://vertexschool.instructure.com/courses/203/files/16083/preview?verifier=EEnbRJTtomcGrdcfJDFKE61QajjNMTbPHucGkIyy" alt="exbake_04.jpg" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/16083" data-api-returntype="File"></p>
<p style="text-align: left;">&nbsp;</p>
<p style="padding-left: 40px;"><span>15. Press "Select" and choose the low poly fbx that is NOT “exploded” and press OK.</span></p>
<p style="text-align: left;">&nbsp;</p>
<p style="text-align: left;"><img src="https://vertexschool.instructure.com/courses/203/files/16084/preview?verifier=ZHPtEZDwV1ZVgHoALPQsAUGjrsz3YoTLL9AkvLUn" alt="exbake_05.jpg" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/16084" data-api-returntype="File"></p>
<p style="text-align: left;">&nbsp;</p>
<p style="text-align: left;"><span>This process enables you to make adjustments to your low poly model and preserve the baked maps, assuming the UV layout has not changed.&nbsp; While one can always bake by mesh name, there is still a risk of the normals being affected by touching or intersecting geometry. So if you have complex models and/ or many close objects the “exploded” method can save you time and stress!</span></p>
</div>
</div>
</div>
</div>