## 三角形图标CSS实现

### HTML
    <div class="triangle"></div>

#### CSS
    .triangle{
       width: 11px;
       position: relative;
       border: none;
       border-top: 15px solid #000;
       border-left: 15px solid #fff;
       border-right: 15px solid #fff;
       margin: 50px;
    }
    .triangle:before{
       content: '';
        display: inline-block;
        width: 15px;
        height: 15px;
        background-color: #000;
        border-radius: 50px;
        position: absolute;
        top: -13px;
        left: -2px;
    }

