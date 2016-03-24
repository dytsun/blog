
![volume.png][1]

;(function() {
  'use strict';

  angular
    .module('sample-app')
    .controller('DynamicController', DynamicController);

  DynamicController.$inject = ['$state'];

    activate();

    function activate(){
      // var drawLine=drawLine;
      var canvasAudio=document.getElementById('canvasAudio');
      var context = canvasAudio.getContext('2d');
      context.beginPath();
      context.strokeStyle='#fff';
      context.lineJoin="round";//圆角
      context.lineWidth=6;
      context.moveTo(50,50);    
      context.lineTo(50,80);
      context.lineTo(80,80);
      context.lineTo(110,110);
      context.lineTo(110,20);
      context.lineTo(80,50);
      context.lineTo(50,50);
      context.closePath();
      context.stroke();

      context.beginPath();
      context.lineCap = 'round';//线条末端样式
      context.moveTo(130,85);
      context.quadraticCurveTo(140,65,130,55);//曲线
      context.stroke();

      context.beginPath();
      context.lineCap = 'round';//线条末端样式
      context.moveTo(150,30);
      context.quadraticCurveTo(170,65,150,100);
      context.stroke();
    } 



  }

})();

 [1]: https://github.com/moondyt/blog/blob/master/pic_volume.png
