# Rainbow Gradient Event List Widget with Animated "Glitter" Effect
Custom CSS for event list widgets that can be copied and pasted into the Streamlabs code editor

https://user-images.githubusercontent.com/75779842/186792798-eb10efbf-bde3-4a51-966c-306eb895e5e5.mov

### 1. Copy the CSS code below

![ezgif com-gif-maker (3)](https://user-images.githubusercontent.com/75779842/186799330-7ffdc973-6b74-4c9e-9331-fcd60b463668.gif)

### 2. Make sure custom HTML/CSS is enabled in your Streamlabs event list dashboard

<img width="455" alt="Screen Shot 2022-08-25 at 8 13 19 PM" src="https://user-images.githubusercontent.com/75779842/186802029-3c3337eb-f833-4459-9f8e-c5b778fd7112.png">

### 3. Paste the code into the CSS section of the Streamlabs code editor (replace any pre-existing code)

![ezgif com-gif-maker (4)](https://user-images.githubusercontent.com/75779842/186803824-ca8deb75-6d3d-467e-8cf1-4c493a48cc3d.gif)


## The CSS Code

```
@import url('https://fonts.googleapis.com/css2?family=Silkscreen&display=swap');

html, .widget-EventList li > div {
    
}

.widget-EventList, .widget-EventList * {
    box-sizing: border-box;
  	text-shadow: 4px 4px 12px #333;
}

.widget-EventList {
    font-weight: 700;
    font-size: 40px;
    font-family: 'Silkscreen', 'sans-serif';
    color: #ebf9ff;
    overflow: hidden;
    list-style: none;
    padding: 0;
    text-transform: uppercase;
    position: relative;

}

.widget-EventList li {
    width: 100%;
    position: relative;
  	-webkit-animation: myAnim 1.5s ease-in 0s 1 normal;
  					animation: myAnim 1.5s ease-in 0s 1 normal;
}

@-webkit-keyframes myAnim {
	0% {
		transform: translateY(-15px);
	}

	100% {
		transform: translateY(0px);
	}
}

@keyframes myAnim {
	0% {
		transform: translateY(-15px);
	}

	100% {
		transform: translateY(0px);
	}
}
.widget-EventList li > div:first-child {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border-radius: 10px;
  	border: 3px solid rgba(235, 249, 255, 0.75);
    opacity: 0.7;
    -webkit-transition: opacity 0.5s linear 2s;
            transition: opacity 0.5s linear 2s;
}

.widget-EventList li > div:last-child {
    overflow: hidden;
    position: relative;
    margin-bottom: 4px;
    padding: 0 10px;
    opacity: 0.7;
    font-size: 0.9em;
    height: 1.2em;
    line-height: 1.2em;
}

.widget-EventList li:first-child > div:first-child {
    opacity: 1;
}

.widget-EventList li:first-child > div:last-child {
    -webkit-animation: growA 1.5s forwards;
  					animation: growA 1.5s forwards;
}


@-webkit-keyframes growA {
    0% {
        opacity: 0;
        font-size: 0em;
        height: 0em;
        line-height: 0em;
        margin-bottom: 0px;
        padding: 0;
    }

    100% {
        opacity: 1;
        font-size: 1em;
        height: 1.6em;
        line-height: 1.6em;
        margin-bottom: 4px;
        padding: 0 10px;
    }
}


@keyframes growA {
    0% {
        opacity: 0;
        font-size: 0em;
        height: 0em;
        line-height: 0em;
        margin-bottom: 0px;
        padding: 0;
    }

    100% {
        opacity: 1;
        font-size: 1em;
        height: 1.6em;
        line-height: 1.6em;
        margin-bottom: 4px;
        padding: 0 10px;
    }
}

.widget-EventList .tag {
    font-size: 0.6em;
    line-height: 0.6em;
    top: 0.4em;
    right: 0.3em;
    position: absolute;
}

.widget-EventList .message {
    padding-right: 3em;
    display: block;
    overflow: hidden;
    white-space: nowrap;
    text-overflow: ellipsis;
}

.widget-EventList li {
    text-shadow: 0 0 1px rgba(0, 0, 0, 0.7), 0 0 2px rgba(0, 0, 0, 0.7), 0 0 3px rgba(0, 0, 0, 0.7);
}

.widget-EventList li > div:first-child {
  	
    background: url("https://raw.githubusercontent.com/redstarblanket/event-list-widget/dank/snowfall-glitter.gif"), linear-gradient(90deg, rgba(255,117,174,1) 0%, rgba(252,163,132,1) 15%, rgba(246,230,154,1) 32%, rgba(187,250,165,1) 50%, rgba(126,230,249,1) 67%, rgba(104,138,251,1) 83%, rgba(165,131,255,1) 100%);
}
```


[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/O4O5BY0J2)



