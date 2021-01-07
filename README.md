# Handbook 📚


## Technical setup

#### Engine: `v12.16.*`
#### React-version `=<16.8`
#### AWS CLI `2`
#### npm `6.14.*`
#### amplify cli `~4.27.2`


## Design
Project should uses the [Atomic design](https://bradfrost.com/blog/post/atomic-web-design/).

### Components
 - All Components must be in a file that starts with a capital letter. (Fx: `BlueButton.tsx`)
 - `atoms` should be files that are purely styled components 
 - `molecules` are components that are small, but contain more than just styled components
 - `organisms` are more complex components that contain multiple molecules/atoms

 ### Pages
 - All pages should have a folder inside content that encapsulates page specific code.

 
## Code Style
Per default do not use eslint or equivilant. Hover some projects will use eslint locally or on 'Git-Commit-Time'.

 - Do not outcomment code. Use the vcs! If you commit regualraly, you can always go back and find old code.
 - Try to make the code compact. Do not have lines with one symble. Fx:
 
 ```html
//Illegal 
<a 
    href="https://www.facebook.com/fundbrickscompany/"
    rel="nofollow noopener"
> 
    <FBIcon 
        name={"facebook"}
    />
</a> 

//Legal 
<a href="https://www.facebook.com/fundbrickscompany/" rel="nofollow noopener"><FBIcon name={"facebook"} /></a>

```

## Security 🛡
Never ever enclude any .env files, api keys or equvilant
