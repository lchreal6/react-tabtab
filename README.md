# react-tabtab

react-tabtab is another react tab. But why you need another react tab?

Some react tabs provide so powerful function like only render the active tab to the DOM or it seperates the tab and panel.

But in my case, I only need the tab that can hide and show. Besides, all the content in the panel is directly render to DOM. That's it. That is react-tabtab.

No other magic. Maybe it would fit in your case.

## Usage

Now only available the commonjs module.

Install it with npm.

    npm install react-tabtab --save

Simple example:

    var Tabs = require('react-tabtab').Tabs;
    var Panel = require('react-tabtab').Panel;

    var App = React.createClass({
      render: function() {
        return (
          <Tabs>
            <Panel title="hi">
              Hi!
            </Panel>
            <Panel title="yo">
              yo yo
            </Panel>
          </Tabs>
        )
      }
    })

    React.render(<App/>, document.getElementById('container'));


## API
    
    | property       | type     | default | required | description                   |
    |----------------|----------|---------|----------|-------------------------------|
    | activeKey      | int      | 0       | no       | set the active key of the tab |
    | handleTabClick | function | n/a     | no       |                               |


## Style

now only use css as style.

if you want to use the same style as teh [demo](), just clone the `dist/tab.css` and inlcude in you project.

    

## License

MIT
