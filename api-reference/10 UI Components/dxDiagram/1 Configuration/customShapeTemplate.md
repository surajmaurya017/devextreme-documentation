---
id: dxDiagram.Options.customShapeTemplate
type: template
---
---
##### shortDescription
Specifies a custom template for shapes.

##### param(container): dxSVGElement
#include common-ref-elementparam with { element: "shape" }

##### param(data): Object
Information about the currently processed shape.

##### field(data.item): dxDiagramShape
The processed shape's object.

##### return: void
<!-- Description goes here -->

---
The template content must be presented as SVG elements.

Use the [template](/api-reference/10%20UI%20Components/dxDiagram/1%20Configuration/customShapes/template.md '/Documentation/ApiReference/UI_Components/dxDiagram/Configuration/customShapes/#template') property to define a template of an individual shape.

[note]

If the [textExpr](/api-reference/10%20UI%20Components/dxDiagram/1%20Configuration/nodes/textExpr.md '/Documentation/ApiReference/UI_Components/dxDiagram/Configuration/nodes/#textExpr') option is specified, template content may overlap with text from the data source. 

Since the [textExpr](/api-reference/10%20UI%20Components/dxDiagram/1%20Configuration/nodes/textExpr.md '/Documentation/ApiReference/UI_Components/dxDiagram/Configuration/nodes/#textExpr') option has the default value `'text'`, the widget will obtain node texts from the data source’s 'text' field. To prevent his behavior, set the option to an empty string: `nodes: { textExpr: "", ...`.

[/note]

#include common-demobutton with {
    name: "Templates",
    url: "https://js.devexpress.com/Demos/WidgetsGallery/Demo/Diagram/CustomShapesWithTemplates/"
}
#include common-demobutton with {
    name: "Templates with Editing",
    url: "https://js.devexpress.com/Demos/WidgetsGallery/Demo/Diagram/CustomShapesWithTemplatesWithEditing/"
}

#####See Also#####
- [Custom Templates](/concepts/05%20UI%20Components/zz%20Common/30%20Templates/10%20Custom%20Templates.md '/Documentation/Guide/UI_Components/Common/Templates/#Custom_Templates')