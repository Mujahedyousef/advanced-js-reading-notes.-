 [Login and Auth Live Url](https://mujahedyousef.github.io/advanced-js-reading-notes.-/day_23/class_23.html)

# Login and Auth

-----

## ROLE-BASED ACCESS CONTROL (RBAC)

* Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control.

* The roles in RBAC refer to the levels of access that employees have to the network.

* Employees are only allowed to access the information necessary to effectively perform their job duties.

### The designations in an RBAC tool can include

* Management role scope – it limits what objects the role group is allowed to manage.
* Management role group – you can add and remove members.
* Management role – these are the types of tasks that can be performed by a specific role group.
* Management role assignment – this links a role to a role group.

### options for user access include

* Primary – the primary contact for a specific account or role.
* Billing – access for one end-user to the billing account.
* Technical – assigned to users that perform technical tasks.
* Administrative – access for users that perform administrative tasks.

### BENEFITS OF RBAC

1. Reducing administrative work and IT support.
1. Maximizing operational efficiency.
1. Improving compliance.

### BEST PRACTICES FOR IMPLEMENTING RBAC

* Current Status
* Current Roles
* Write a Policy
* Make Changes
* Continually Adapt

----
## react-cookies

* Install
```
$ npm install react-cookies --save
```
* Usage
```
import { Component } from 'react'
import cookie from 'react-cookies'
 
import LoginPanel from './LoginPanel'
import Dashboard from './Dashboard'
 
class MyApp extends Component {
  constructor () {
    super()
 
    this.onLogin = this.onLogin.bind(this)
    this.onLogout = this.onLogout.bind(this)
  }
 
  componentWillMount() {
    this.state =  { userId: cookie.load('userId') }
  }
 
  onLogin(userId) {
    this.setState({ userId })
    cookie.save('userId', userId, { path: '/' })
  }
 
  onLogout() {
    cookie.remove('userId', { path: '/' })
  }
 
  render() {
    const { userId } = this.state
 
    if (!userId) {
      return <LoginPanel onSuccess={this.onLogin} />
    }
 
    return <Dashboard userId={userId} />
  }
}


```
-----
[react-cookies component](https://www.npmjs.com/package/react-cookies)


[react-cookie library](https://www.npmjs.com/package/react-cookie)




