# React Scroll Sensor

## Docs are still under development

Wanna create animated sites when they get scrolled, read on,

 > TLDR; Unopiniated sensor to detect when your component gets into the viewport and inject the intersection info into your component.

 If you ever have tried to implement the support necessory to detect when your components gets into the viewport when scrolling, you know how much it hurts. That's the exact reason this library is here.
 Whether you want to use scroll event based tracking or intersection observer based tracking, it's already packed into this sensor.

> Not TLDR;

 What this library expose is a flexible toolkit for detecting viewport intersecting. What you do with it completely up to you. Also we dont use this.props.children, but HOCs. We follow redux style to architect the library. Basically we have a provider and a connector. Provider contains the detection algorithm and connector used to connect your components to the provider. This way we can swap the implementation in config without changing the code in same connector types.
