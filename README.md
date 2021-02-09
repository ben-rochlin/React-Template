# React-blank-Template
Blank react template to be used in place of create-react-app.

## Purpose
There are several configurations and settings that I would like to use across all my react applications, this template will be used as a blank canvas to get my react apps up and running quickly and allow me to focus on actually coding.

## Features

- Global CSS reset/config file

    A global css file to reset default styles from web browsers and to provide a simple entry point for global styles which can be accessed by each component.

- locally scoped SCSS

    Which allows me to use scss classnames that will only be applied to the elements contained within the file that the scss is imported into, I can reuse the same scss class names throughout my application by simply naming the scss file `example.scoped.scss` and not have to worry about styles overiding other components/elements with the same class name. click [here](https://dev.to/viclafouch/how-to-scope-your-css-scss-in-react-js-271a) for more info.
    
- Babel Module resolver for easier relative paths

    which will allow for much simpler file/function imports from relative paths with the use of an alias in place of cumbersome relative paths. click [here](https://www.robinwieruch.de/babel-module-resolver) for more info. 
    
    Example:
    
      // old way to import
      import { CheckIcon } from '../components/icons'
      import CancelIcon from '../components/icons/CancelIcon'
 
      // new way to import
      import { CheckIcon } from '@icons'
      import CancelIcon from '@icons/CancelIcon'
      
   
    
    
    
- Folder/File structure
    
    My preference for how I would like my folders and files to be structured within my application. components, pages, routes, services ect
