# Understanding Low Poly Modeling

<p><iframe src="https://player.vimeo.com/video/452915573" width="960" height="540" allowfullscreen="allowfullscreen" allow="autoplay; fullscreen"></iframe></p>
<p>&nbsp;</p>
<h2><span>Low Poly in Today’s Industry</span></h2>
<p><span>As hardware has grown more powerful and software has grown more efficient, each generation we’re able to push the boundaries further and further. One big pitfall that many beginning game artists get caught up by is the level of detail expected in the game resolution mesh.&nbsp;</span></p>
<p><span>There is one big topic that always seems to be glaring us in the face:</span></p>
<p><strong>Polycount (or Triangle Count)</strong></p>
<p><span>It’s a scary topic that stems from the limitations of hardware in the early days of 3D games. But as each generation of hardware has hit the consumer market, we’ve been able to push further and further. The reality is that you can generally push your low poly a lot further than you might think you can.</span></p>
<p>&nbsp;</p>
<h2><span>Don’t Get Stuck in 2005</span></h2>
<p><img src="https://vertexschool.instructure.com/courses/203/files/16071/preview?verifier=XNDKMkE3OhaxscwqpuWuo9TxKLtMtrK9aoVIJoea" alt="lp-stuck-2005.jpg" width="800" height="436" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/16071" data-api-returntype="File"></p>
<p><span>Many beginning game artists tend to get stuck in the idea that the current limitations for game art are the same as they were in previous generations. The instinct is to try to hit triangle counts that were typical of games from the PS3/XBox 360 era of games. Then they will get frustrated when their art doesn’t look as good as what they see in current gen games.</span></p>
<p><span>This is partly due to a wealth of information and forum posts on the internet from that era about triangle counts. As hardware has advanced, we’re able to push the triangle counts even further. With that evolution comes less conversation about triangle counts in general.&nbsp;</span></p>
<p><span>Let’s ask a question across a 15 year span:</span></p>
<p><strong>How many triangles should a low poly barrel have?</strong></p>
<ul>
<li style="list-style-type: none;">
<ul>
<li><strong>Answer in 2005:</strong><span> 300 tris</span></li>
<li><strong>Answer in 2010:</strong><span> 600 tris</span></li>
<li><strong style="font-family: inherit; font-size: 1rem;">Answer in 2020:</strong><span> As many as it takes to capture the silhouette</span></li>
</ul>
</li>
</ul>
<p>&nbsp;</p>
<table style="border-collapse: collapse; width: 100%;" border="1">
<tbody>
<tr>
<td style="width: 100%;">
<h2 style="padding-left: 40px;"><span>Real World Examples of Exponential Growth</span></h2>
<p style="padding-left: 40px;"><img src="https://vertexschool.instructure.com/courses/203/files/16079/preview?verifier=VWyBNTmVrxp0w1QNS8edPXKJ52m7QQ2WfGa6xynL" alt="GOW-evolution.jpg" width="600" height="338" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/16079" data-api-returntype="File"></p>
<p style="padding-left: 40px;"><span>Let’s have a look at the evolution of Kratos from the God of War series.</span></p>
<ul>
<li style="list-style-type: none;">
<ul>
<li style="list-style-type: none;">
<ul>
<li><strong>God of War 2 (PS2):</strong><span> 5700 triangles with gear</span></li>
<li><strong>God of War 3 (PS3):</strong><span> 64,000 triangles with gear</span></li>
<li><strong>God of War 2018 (PS4):</strong><span> 80,000 triangles without gear (up to 120k with gear)</span></li>
</ul>
</li>
</ul>
</li>
</ul>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p><span>As you can see by the numbers from God Of War above, triangle count budgets have skyrocketed through the generations. Pushing the boundaries makes sense for main characters, but what about our props?</span></p>
<p><span>The main lesson to walk away with is that </span><strong>you shouldn’t get too hung up on triangle counts</strong><span>. Build whatever geometry is needed to</span><strong> capture the silhouette</strong><span>.&nbsp;</span></p>
<p><span>&nbsp;</span></p>
<h2><span>Capturing the Silhouette</span></h2>
<p><strong>Wait… what is a silhouette???</strong></p>
<p><span><img src="https://vertexschool.instructure.com/courses/203/files/16073/preview?verifier=GPEQTitG0bDr1Yj97USyGOGef3R753rzPeb4RKhk" alt="what-is-silhouette-1.jpg" width="500" height="382" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/16073" data-api-returntype="File"><br></span></p>
<p><span>When we say build whatever it takes to capture the silhouette, that means </span><strong>the low poly geometry should capture the shape of the high poly</strong><span>. We build it like a shell around the high poly.</span></p>
<p><span>The low poly should have just enough geometry to capture the high poly’s silhouette shape. </span><span><br><br></span></p>
<p><img src="https://vertexschool.instructure.com/courses/203/files/16074/preview?verifier=dtbVjVlRUKcV44kdhGegePHxOObKbLijmAHqHka4" alt="silhouette-example.jpg" width="800" height="450" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/16074" data-api-returntype="File"></p>
<p><span>We should still be mindful of performance, however. Where the high poly is made of separate pieces and has all the detail, the low poly should be made of as few pieces as possible. We build it like a shell around the high poly.</span></p>
<p><span><br><img src="https://vertexschool.instructure.com/courses/203/files/16075/preview?verifier=rbB96Ey3GGuPLT0qxtRLGFMBfJpm04CDFUI9U3az" alt="lp-shell-over-hp.jpg" width="500" height="388" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/16075" data-api-returntype="File"><br></span></p>
<p>&nbsp;</p>
<h2><span>Tip #1: No More Hard Edges</span></h2>
<p><span>With increased polycount budgets and better baking tools, we want to make sure that we avoid hard 90 degree edges wherever possible. By beveling the edges of our low poly model, we’ll get cleaner bakes and less texture seams.&nbsp;</span></p>
<p><img src="https://vertexschool.instructure.com/courses/203/files/16077/preview?verifier=fl17VFhbM5DjDtGGE6DO91m6xKQ70d69YhWq8daU" alt="bevel-edges-bake.jpg" width="600" height="338" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/16077" data-api-returntype="File"></p>
<p><img src="https://vertexschool.instructure.com/courses/203/files/16078/preview?verifier=mUDxdJMMc9nTG2YFVshB2Ymei7fHXTcSbsiADvK9" alt="bevel-edges-bake02.jpg" width="600" height="289" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/16078" data-api-returntype="File"></p>
<p>&nbsp;</p>
<h2><span>Tip # 2: Save On The Straights, Spend on the Curves</span></h2>
<p><span>Triangles are no longer an expensive limitation, but we do still have to be mindful of how much geometry we are using. We’re able to push the geometry further, but with hundreds of objects on screen at a time, that all still adds up.</span></p>
<p><span>A very important technique we can use to take control of our triangle budgets while still capturing the silhouette of our high poly is to always remember that we <strong>save on the straights so we can spend on the curves</strong>. This means we should avoid any additional edges or vertices that don’t change the silhouette, such as along a planar surface with straight edges. But we want to always spend whatever geometry is necessary to properly capture every curve.</span></p>
<p><img src="https://vertexschool.instructure.com/courses/203/files/16076/preview?verifier=VpzouprZYqmUSsmDEUfuY337S8XjNdZDlhq331Sb" alt="save-straights-spend-curves.jpg" width="800" height="450" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/203/files/16076" data-api-returntype="File"></p>
<hr>