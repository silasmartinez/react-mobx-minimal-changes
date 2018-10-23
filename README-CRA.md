## Decorators and Mobx
This project contains the changes required to enable a typical app
bootstrapped with create-react-app to leverage decorators, which
are, IMO, the easiest to read way of implementing mobx.

Modern mobx does contain strong support for emulating decorator 
functionality, but still requires a fair amount of boilerplate.

### Of note:
package.json changes include:
* npm dependencies (mobx, babel decorator support, and react-app-rewired support)
* yarn script changes

config.overides.js is a new file, leveraged by react-app-rewired,
which enables (legacy) decorator support for babel, as called by
webpack.
