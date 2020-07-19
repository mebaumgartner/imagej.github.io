{{Infobox
| software               = ImageJ
| name                   = Shape Index Map
| maintainer             = {{Person|Schindelin}}
| author                 = Johannes Schindelin
| source                 = {{GitHub|org=fiji|repo=Fiji_Plugins|source=fiji/geom/Shape_Index_Map.java}}
| released               = 18/08/2010
| latest version         = 18/08/2010
| status                 = 
| category               = [[:Category:Plugins]]
| website                = 
}}

== Explanation ==

The [http://journals.cambridge.org/action/displayAbstract?fromPage=online&aid=6820324 shape index] describes the surface topology of the image interpreted as a [[3D Surface Plot|height field]]:

{| border="1"
|-
|+ shape index
| 1
| 0.75
| 0.5
| 0.25
| 0
| -0.25
| -0.5
| -0.75
| -1
|-
|+ meaning
| cap
| dome
| ridge
| saddle ridge
| saddle
| saddle rut
| rut
| trough
| cup
|}

The shape index is calculated from the principal curvatures of the Hessian, which is very susceptible to noise. Therefore the plugin asks you to specify a radius for Gaussian blurring as a preprocessing step.

== Example ==

[[Image:Shape_Index-orig.jpg]]

With radius 2, this results in the following shape index map (bright spots correspond to caps, dark to cups):

[[Image:Shape_Index-map.jpg]]

[[Category:Plugins]]