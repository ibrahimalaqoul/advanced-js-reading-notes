## Redux Toolkit
The Redux Toolkit package is intended to be the standard way to write Redux logic. It was originally created to help address three common concerns about Redux:

"Configuring a Redux store is too complicated"
"I have to add a lot of packages to get Redux to do anything useful"
"Redux requires too much boilerplate code"
We can't solve every use case, but in the spirit of create-react-app, we can try to provide some tools that abstract over the setup process and handle the most common use cases, as well as include some useful utilities that will let the user simplify their application code.

Redux Toolkit also includes a powerful data fetching and caching capability that we've dubbed "RTK Query". It's included in the package as a separate set of entry points. It's optional, but can eliminate the need to hand-write data fetching logic yourself.

These tools should be beneficial to all Redux users. Whether you're a brand new Redux user setting up your first project, or an experienced user who wants to simplify an existing application, Redux Toolkit can help you make your Redux code better.

## MobX
MobX is a simple, scalable and battle tested state management solution. This tutorial will teach you all the important concepts of MobX in ten minutes. MobX is a standalone library, but most people are using it with React and this tutorial focuses on that combination.

The core idea
State is the heart of each application and there is no quicker way to create buggy, unmanageable applications than by producing an inconsistent state or state that is out-of-sync with local variables that linger around. Hence many state management solutions try to restrict the ways in which you can modify state, for example by making state immutable. But this introduces new problems; data needs to be normalized, referential integrity can no longer be guaranteed and it becomes next to impossible to use powerful concepts like classes in case you fancy those.

MobX makes state management simple again by addressing the root issue: it makes it impossible to produce an inconsistent state. The strategy to achieve that is simple: Make sure that everything that can be derived from the application state, will be derived. Automatically.

Conceptually MobX treats your application like a spreadsheet.
## Hookstate
Intuitive API. Most things will be self-explanatory. More in depth description will always be there.
Code samples in each section are self-contained, complete and interactive. So, jump to the relevant section, copy-paste a sample to your app and extend it as needed.
Intellisense by IDE. If your project is in Typescript, you will benefit a lot as type inference of the API functions supports any complexity of data structures of your states. Of course, you can also use it from plain javascript.
Complete demo application. There is a Todo-list-like complete demo application built with Hookstate. It uses and demonstrates most of the core features of Hookstate. It gives an example of how to organise your project. You may follow the example or use any other module-composition structure. Here it is running in an iframe: