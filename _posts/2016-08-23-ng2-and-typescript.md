---
layout: post
title: Angular2 and Typescript
---

Several weeks ago, our development team here at iOffice began the monumental task of preparing for Angular2/Typescript development. There has been shouting. And tears. And a significant increase in chocolate consumption. Our team has bonded in hatred of the angular core team with each breaking change and gushed as interesting new features and fixes actually become available.

Once our build process stabilized and we cemented the the integration with our existing Angular1 code, I started on one of our two new Angular2 projects. I found getting started to be extremely difficult, so I've decided to write this post and keep a running list of blogs, links and tools that have made my life easier.


_Useful resources:_

  * [ui-router for Angular2 example](https://github.com/ui-router/quickstart-ng2)
  * [AiA Angular 2 Tips podcast with Pascal Precht](https://devchat.tv/adv-in-angular/097-aia-angular-2-tips-with-pascal-precht) - my introduction to @ViewChildren and @ContentChildren
  * [Angular2 video course](https://frontendmasters.com/courses/angular-2/) - I only caught the first few hours of this course from Frontend Masters before my account expired :(
  * [NG2/TS Live Templates for IntelliJ IDEA](https://plugins.jetbrains.com/plugin/8395?pr=idea)
  
_Gotchas:_

  * Doing `*ngFor` with a list of objects and passing the entire object when selected not currently possible
  * [Pipes don't work in Safari](https://github.com/angular/angular/issues/3333)
