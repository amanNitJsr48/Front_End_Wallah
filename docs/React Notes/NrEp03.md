## Namaste react episode3 notes

### Q: Why should we use key inside a map function ?
React optimizes the render cycle to reduce unnecessary re-rendering. When using the .map() function to render a list of components, if we don't provide a unique key for each component, React will re-render all components in the list whenever there's any update or a new component is added. This happens because, without unique keys, React can't differentiate between components, so it clears the entire list and renders it again with the latest data.

On the other hand, by assigning a unique key to each component in the list, React can identify which components have changed, been added, or removed. As a result, only the new or updated components are rendered, reducing the rendering load and making the app faster.

Note: Some people also use index as a key but never use index as a keys..learn react bad practices

### What is configdriven UI ?
onfig-driven UI is a design approach where the user interface (UI) is dynamically controlled and rendered based on external configuration data rather than hard-coded UI logic. This means that changes in UI elements, behaviors, or displayed content can be made simply by modifying a configuration file, database entries, or an API response, without altering the application’s underlying code.

Key Points of Config-Driven UI:
* Dynamic UI Changes: The UI adapts based on data inputs, so different configurations can lead to different UIs or behaviors without changing the core code.
* Customizable and Scalable: Config-driven UI is highly useful for large applications where different regions, user roles, or user preferences may require different UI experiences. It allows a single codebase to support diverse UI requirements.
* Easier Updates: Modifying the configuration data can lead to instant changes in the UI, which is faster and more manageable than redeploying the code every time.<br />
#### Example - Zomato:
Take Zomato, which offers a food ordering interface. The same UI may look different across various locations due to config-driven design:

* Location-Based Offers: If Zomato has specific offers in Mumbai but not in Delhi, the configuration data fetched for each location will determine what offers to show.
* Custom Content: Different restaurants, discounts, and availability are displayed based on the user’s location, all controlled by configuration data.
* Seasonal Themes or Promotions: Zomato can update themes or offer banners during events (e.g., Diwali promotions) by changing the configuration rather than modifying the code.

#### NOTE:-
 * passing props to a react component is just like passing arguments to a function bcz React component is at the end of the day a Javascript function.
 * all the props are wrap in a object and passed to component
 * when you have to pass data dynamically to a component then pass it as a props 
 * config driven UI - controlling your UI based on data. Ex - same Zomato UI will show different UI or offers for diffrenet location based on data
 * Read [array map,reduce and filter](https://www.youtube.com/watch?v=zdp0zrpKzIE) as well as [higher order function](https://www.youtube.com/watch?v=HkWxvB1RJq0)
 * Read what is cloudinary CDN
 * 
 