# Babel Standalone Demo

[![Netlify Status](https://api.netlify.com/api/v1/badges/732cc95c-d68a-47de-ace4-f1ce59512b35/deploy-status)](https://app.netlify.com/sites/babel-standalone/deploys)

https://babel-standalone.netlify.app/

This is just a quick demo to show how [@babel/standalone](https://babeljs.io/docs/en/babel-standalone) works. All we have is an html file. That file loads React, ReactDOM, and @babel/standalone through script tags.

We can then write our next-gen JavaScript directly in the html file and it will work! Pretty cool.

How does this work? If we inspect the DOM through Chrome DevTools, we can see that our original jsx code is right where it was, in the script tag before the closing tag of the body. But if we take a look at the head, we can see that another script tag was added! This is the compiled JavaScript, and we can see that we now have the raw React APIs like createElement.

Note that this kind of approach is not recommended for production. Nevertheless, it might be valuable for quick proof of concepts, tutorials, or education purposes.
