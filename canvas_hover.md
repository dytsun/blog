
> var canvas = document.getElementById("canvas");

> var ctx = canvas.getContext("2d");

> var canvasOffset = $("#canvas").offset();

> var offsetX = canvasOffset.left;

> var offsetY = canvasOffset.top;

> var myCircle = {
>     x: 150,
>     y: 150,
>     radius: 25,
>     rr: 25 * 25, // radius squared
>     hovercolor: "red",
>     blurcolor: "green",
>     isHovering: false
> }

> function drawCircle(circle) {
>     ctx.beginPath();
>     ctx.arc(circle.x, circle.y, circle.radius, 0, Math.PI * 2);
>     ctx.closePath();
>     ctx.fillStyle = circle.isHovering ? circle.hovercolor : circle.blurcolor;
>     ctx.fill();
> }

> drawCircle(myCircle);

> function handleMouseMove(e) {
>     mouseX = parseInt(e.clientX - offsetX);
>     mouseY = parseInt(e.clientY - offsetY);
>     var dx = mouseX - myCircle.x;
>     var dy = mouseY - myCircle.y;
>     // math to test if mouse is inside circle
>     if (dx * dx + dy * dy < myCircle.rr) {
>         // change to hovercolor if previously outside
>         if (!myCircle.isHovering) {
>             myCircle.isHovering = true;
>             drawCircle(myCircle);
>         }
>     } else {
>         // change to blurcolor if previously inside
>         if (myCircle.isHovering) {
>             myCircle.isHovering = false;
>             drawCircle(myCircle);
>         }
>     }
> }

> $("#canvas").mousemove(function (e) {
>     handleMouseMove(e);
> });
