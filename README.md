# POST-Geoserver

###### Request type Point 
```
Point = `<wfs:GetFeature service="WFS" version="1.0.0"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xsi:schemaLocation="http://www.opengis.net/wfs"
    xmlns:gml="http://www.opengis.net/gml" xmlns:wfs="http://www.opengis.net/wfs"
    xmlns:ogc="http://www.opengis.net/ogc">
    <wfs:Query typeName="yopal:gc_predios_catastro">
        <ogc:Filter>
            <ogc:Intersects>
                <ogc:PropertyName>geom</ogc:PropertyName>
                <gml:Point>
                    <gml:coordinates>-72.38535032735483,5.304119233718497</gml:coordinates>
                </gml:Point>
            </ogc:Intersects>
        </ogc:Filter>
    </wfs:Query>
    </wfs:GetFeature>`
```
###### Request type Polygon
```
Polygon = `<wfs:GetFeature service="WFS" version="1.0.0"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xsi:schemaLocation="http://www.opengis.net/wfs"
    xmlns:gml="http://www.opengis.net/gml" xmlns:wfs="http://www.opengis.net/wfs"
    xmlns:ogc="http://www.opengis.net/ogc">
    <wfs:Query typeName="yopal:gc_predios_catastro">
        <ogc:Filter>
            <ogc:Intersects>
                <ogc:PropertyName>geom</ogc:PropertyName>
                <gml:Polygon srsName="http://www.opengis.net/gml/srs/epsg.xml#4326">
                        <gml:outerBoundaryIs>
                            <gml:LinearRing>
                                <gml:coordinates decimal="." cs="," ts=" ">
                                -72.39706725786893,5.308014035017205
                                -72.39723623935087,5.307819051231754
                                -72.39693046333595,5.307720223810079
                                -72.39681780901466,5.307917878637552
                                -72.39706725786893,5.308014035017205
                                </gml:coordinates>
                            </gml:LinearRing>
                        </gml:outerBoundaryIs>
                </gml:Polygon>
            </ogc:Intersects>
        </ogc:Filter>
    </wfs:Query>
    </wfs:GetFeature>`
```
