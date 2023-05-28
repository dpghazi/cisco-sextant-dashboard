# Cisco Sextant Dashboard App
## **Project Description**
- The Sextant Networking Dashboard is a single-page application meant to assist field technicians with their day-to-day tasks. 
- This web application uses <a href="https://github.com/facebook/create-react-app" target="_blank">React</a> for the frontend to display the user’s public IP addresses (both ipv4 and ipv6) and the packet latency associated with a service called <a href="https://www.npmjs.com/package/pylon" target="_blank">Pylon</a>. 
- The user's public IP addresses are fetched from the <a href="https://www.ipify.org/" target="_blank">ipify API</a> and the packet latency can be streamed using <a href="https://www.npmjs.com/package/websocket" target="_blank">WebSocket connections</a>.

### **Overview**

- **Designing the Sextant Frontend**
  - Created a banner component at the top of the page which displays the site’s title.
  - Created an exhibit component that displays a heading.
  - Created child components which wrap the components to logically separate different data points.
- **Displaying the User's Public IP**
  - Created a new component to collect and display the user’s public IP addresses.
    - The component makes an HTTP request to the ipify API as soon as it is mounted and surface the resultant data to the user.
    - The component accepts a prop that determines whether it requests an ipv4 address or an ipv6 address.
  - Added two instances of this component to the page, both wrapped in an exhibit component from the last task.
    - One displays the user’s ipv4 address, and the other displays the user’s ipv6 address.
- **Streaming Data from a Networked Service**
  - Created a new React Component, which displays packet latency from Pylon.
  - Added the component to my React app, living inside an Exhibit.

## Ticket Result

![Kapture 2022-08-30 at 00 20 15](https://user-images.githubusercontent.com/94224903/187374854-488fcf75-f2d5-49d8-a6c6-d93684955c18.gif)
![Screen Shot 2022-08-30 at 12 16 04 AM](https://user-images.githubusercontent.com/94224903/187374936-d8f874c1-aef8-4be6-b751-6dc06333c3ae.jpg)
                                            *Using VPN to hide personal IP addresses*


### Language **& Tools**

- JavaScript (React.js)
- HTML/CSS
- ipify API
- WebSockets Protocol
- Pylon
