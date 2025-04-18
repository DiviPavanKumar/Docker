<mxfile host="app.diagrams.net" agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/135.0.0.0 Safari/537.36" version="26.2.13">
  <diagram name="Page-1" id="T8dOXnx0VX6JwbCkfarl">
    <mxGraphModel dx="927" dy="491" grid="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="1" pageScale="1" pageWidth="850" pageHeight="1100" math="0" shadow="0">
      <root>
        <mxCell id="0" />
        <mxCell id="1" parent="0" />
        <mxCell id="1gjTNdFsdWmKvrDtKBR6-1" value="" style="whiteSpace=wrap;html=1;aspect=fixed;" vertex="1" parent="1">
          <mxGeometry x="320" y="150" width="260" height="260" as="geometry" />
        </mxCell>
        <mxCell id="1gjTNdFsdWmKvrDtKBR6-2" value="Docker Container&lt;br&gt;Like Nginx, Port: 80" style="rounded=1;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="382.68" y="170" width="120" height="60" as="geometry" />
        </mxCell>
        <mxCell id="1gjTNdFsdWmKvrDtKBR6-9" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;" edge="1" parent="1" source="1gjTNdFsdWmKvrDtKBR6-4" target="1gjTNdFsdWmKvrDtKBR6-2">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="1gjTNdFsdWmKvrDtKBR6-4" value="" style="image;sketch=0;aspect=fixed;html=1;points=[];align=center;fontSize=12;image=img/lib/mscae/Docker.svg;" vertex="1" parent="1">
          <mxGeometry x="400" y="30" width="85.37" height="70" as="geometry" />
        </mxCell>
        <mxCell id="1gjTNdFsdWmKvrDtKBR6-8" value="VM" style="text;html=1;align=center;verticalAlign=middle;resizable=0;points=[];autosize=1;strokeColor=none;fillColor=none;" vertex="1" parent="1">
          <mxGeometry x="470" y="118" width="40" height="30" as="geometry" />
        </mxCell>
        <mxCell id="1gjTNdFsdWmKvrDtKBR6-10" value="HUB" style="text;html=1;align=center;verticalAlign=middle;resizable=0;points=[];autosize=1;strokeColor=none;fillColor=none;" vertex="1" parent="1">
          <mxGeometry x="417.68" width="50" height="30" as="geometry" />
        </mxCell>
        <mxCell id="1gjTNdFsdWmKvrDtKBR6-14" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;entryX=0;entryY=0.5;entryDx=0;entryDy=0;" edge="1" parent="1" source="1gjTNdFsdWmKvrDtKBR6-11" target="1gjTNdFsdWmKvrDtKBR6-2">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="1gjTNdFsdWmKvrDtKBR6-11" value="Server Port: 80" style="whiteSpace=wrap;html=1;aspect=fixed;" vertex="1" parent="1">
          <mxGeometry x="290" y="170" width="60" height="60" as="geometry" />
        </mxCell>
        <mxCell id="1gjTNdFsdWmKvrDtKBR6-13" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;entryX=0;entryY=0.5;entryDx=0;entryDy=0;" edge="1" parent="1" source="1gjTNdFsdWmKvrDtKBR6-12" target="1gjTNdFsdWmKvrDtKBR6-11">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="290" y="200" as="targetPoint" />
            <Array as="points">
              <mxPoint x="240" y="200" />
              <mxPoint x="240" y="200" />
            </Array>
          </mxGeometry>
        </mxCell>
        <mxCell id="1gjTNdFsdWmKvrDtKBR6-20" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;entryX=0;entryY=0.5;entryDx=0;entryDy=0;" edge="1" parent="1" source="1gjTNdFsdWmKvrDtKBR6-12" target="1gjTNdFsdWmKvrDtKBR6-17">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="250" y="290" as="targetPoint" />
            <Array as="points">
              <mxPoint x="230" y="200" />
              <mxPoint x="230" y="290" />
            </Array>
          </mxGeometry>
        </mxCell>
        <mxCell id="1gjTNdFsdWmKvrDtKBR6-12" value="" style="html=1;verticalLabelPosition=bottom;align=center;labelBackgroundColor=#ffffff;verticalAlign=top;strokeWidth=2;strokeColor=#0080F0;shadow=0;dashed=0;shape=mxgraph.ios7.icons.user;" vertex="1" parent="1">
          <mxGeometry x="110" y="170" width="80" height="60" as="geometry" />
        </mxCell>
        <mxCell id="1gjTNdFsdWmKvrDtKBR6-16" value="Another Nginx container: 80" style="rounded=1;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="382.68" y="260" width="120" height="60" as="geometry" />
        </mxCell>
        <mxCell id="1gjTNdFsdWmKvrDtKBR6-22" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;" edge="1" parent="1" source="1gjTNdFsdWmKvrDtKBR6-17" target="1gjTNdFsdWmKvrDtKBR6-16">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="1gjTNdFsdWmKvrDtKBR6-17" value="server port: 8080" style="whiteSpace=wrap;html=1;aspect=fixed;" vertex="1" parent="1">
          <mxGeometry x="290" y="260" width="60" height="60" as="geometry" />
        </mxCell>
      </root>
    </mxGraphModel>
  </diagram>
</mxfile>
