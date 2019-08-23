---
title: "EMF Client Platform"
featured_image: '/images/ecp.png'
description: "Are you still manually coding UIs?"
---
The EMF Client Platform is a framework for building EMF-based client applications. The goal is to provide reusable, adaptable and extensible UI components to develop applications based on a given EMF model. All components can be used stand-alone and be embedded into your own application. To get started, ECP provides a demo application, which integrates all provided components. This demo application allows you to get started by only providing your EMF model.

## Form-Based UI
Many applications require to display and modify entities in a form-based UI. "EMF Forms", a sub project of the EMF Client Platform provides support for this. EMF Forms allows to render a form-based UI for a single entity or several entities. The form-based UI allows the modification of all attributes and references. By default, the UI is rendered reflectively, meaning you can open any entity of your application without any additional adaptations or code generation. If you add new entity types to your model, the EMF Forms will still work out-of-the-box.

EMF Forms can be embedded into any kind of UI, even in dialogs. The demo application shows the integration of EMF Forms as an RCP editor.

Additionally, the EMF Forms shows the result of validation constraints. This way, users are informed about malformed data, e.g. a missing attribute.

EMF Forms highly customizable, it is possible to add custom components (widgets) for certain attributes or references. Additionally EMF Forms allows to customize the layout of the UI and include specific UI customizations, such as rule-based visibility of controls. Customizations can be expressed in a simple model and are interpreted by a rendering component. Therefore you do not have to manually write UI code. The approach is even independant from a UI toolkit, you can migrate your UI to JavaFX or to the Web just by replacing the renderer. EMF Forms allows to customize and optimized form-based UIs for your application. As the relfective default UI still works for all elements you perform customization in small iterative steps. Please see here for more information about EMF Forms.

## One-Click Application
EMF enables the automatic generation of the entity model for an application. Additionally, EMF provides frameworks for a variety of tasks, e.g., to store and collaboratively work on these entities. However, creating a user interface for browsing and modifying entities based on an EMF model still requires a lot of manual work. The same is true for the integration of different storage technologies.

The EMF Client Platform enables you to set up the first version of your own application in less than one minute, just by providing your entity model in EMF. In contrast to the generated editor of EMF, the EMF Client Platform provides not only a generic UI but a highly extensible and adaptable UI to create, modify and share EMF model instances. No manual coding or code generation is required. As a prerequisite, you only need to provide an EMF model plugin describing the entity objects of your application as well as the corresponding edit plugin - both generated from your EMF Ecore model. The EMF Client Platform is able to render its UI reflectively, based only on the information contained in the model.

Since the EMF Client Platform provides a reflective UI, the resulting application is robust against a change in the data model. That means you can evolve the underlying data model without any manual adaptations of the UI. Based on the provided application, the EMF Client Platform is highly customizable. It allows to iteratively add custom pieces to the already running application. Therefore it enables you to develop an application in a very agile manner, maintain a shippable application at any point in time and focus only on the things you want to adapt.