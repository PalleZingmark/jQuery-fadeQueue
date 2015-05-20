#jQuery fadeQueue, v0.5
Dual licensed under the MIT and GPL licenses.

#AUTHOR
Palle Zingmark 
*[info@palleman.nu](info@palleman.nu) 
*[palleman.nu](palleman.nu) 
*[twitter.com/palleman](twitter.com/palleman) 

#DEMOS
*http://jquery.palleman.nu/fadequeue/
*http://jsfiddle.net/pallezingmark/D46fS/

#DESCRIPTION
This plugin creates a queue containing all children inside the
provided parent element, then the plugin steps thru the queue
and fades in the element, one after another. You can also
choose to start the queue at any direct children inside the
provided parent.

```JavaScript
@param {number|object|function} These parameters can be provided:

@param {number} Provide the duration (miliseconds) for the queued item to fade in.
  @default: 200
  @example:
    $('#mydiv').fadeQueue(500);

@param duration [number] {object} Provide the duration (miliseconds) for the queued item to fade in.
  @default: 200
  @example:
    $('#mydiv').fadeQueue({
      duration: 500
    });

@param pause [number] {object} Provide a pause (miliseconds) between the fade in durations.
  @default: (duration / 2)
  @example:
    $('#mydiv').fadeQueue({
      pause: 100
    });

@param startAt [node] {object} Provide a node where the animation will force a start.
  @default: first-child
  @example:
    $('#mydiv').fadeQueue({
      startAt: $('#mydiv :nth-child(3)')
    });

@param {function} Provide a callback function that will be called when queue is empty.
  @example:
    $('#mydiv').fadeQueue(function(){
      alert('Queue is empty')
    });
```