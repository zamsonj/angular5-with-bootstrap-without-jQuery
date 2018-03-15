1. Install Node.js from nodejs.org/en/
2. The npm(node package manager) will come with Node.js.
3. Open the command prompt in your project folder.
4. Install latest version of angular globally by typing 
        npm install -g @angular/cli
5. Create a new angular application by typing 
        ng new a5b4app
6. To run the app go to the folder and type
        ng serve
7. Here we are using ng-bootstrap instead of bootstrap.js and jquery.js
8. You should have the boostrap.css file.
9. Visit http://getbootstrap.com/ and get the cdn link and paste it in the index.html
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">
10. In this example we are testing a nav bar which has some links, a dropdown and a collapse button for small screen.
11. The styles will be applied just by adding the css file.
12. But to have dropdown or collapse to work properly we should install ng-bootstrap which supports all the bootstrap functionalities.
13. Type the statement given below in command prompt. The module will be added into your node_modules folder and package.json will be updated.
        npm install --save @ng-bootstrap/ng-bootstrap
14. Once installed import into our app.module.ts file.
        import {NgbModule} from '@ng-bootstrap/ng-bootstrap';
15. Add 'NgbModule.forRoot()' into the 'import' array.
        @NgModule({
        declarations: [
            AppComponent
        ],
        imports: [
            BrowserModule,
            NgbModule.forRoot()
        ],
        providers: [],
        bootstrap: [AppComponent]
        })
16. To know more about ng-bootstrap and it's directives visit https://ng-bootstrap.github.io/