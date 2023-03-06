# Anti-ad-block-for-blogger

1. Login your blogger
2. Go to theme
3. Edit HTML
4. Find </head> and place below script before </head> tag

```
<style>
    #adblock {
        backdrop-filter: blur(5px);
        background: rgba(0, 0, 0, 0.25);
        padding: 20px 19px;
        border: 1px solid #ebeced;
        border-radius: 10px;
        color: #ebeced;
        overflow: hidden;
        position: fixed;
        margin: auto;
        left: 10;
        right: 10;
        top: 0;
        width: 100%;
        height: 100%;
        overflow: auto;
        z-index: 999999
    }

    #adblock .inner {
        background: #f5f2f2;
        color: #000;
        box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
        text-align: center;
        width: 600px;
        padding: 40px;
        margin: 80px auto
    }

    #adblock button {
        padding: 10px 20px;
        border: 0;
        background: #e9e9e9;
        margin: 20px;
        box-shadow: 0 5px 10px rgba(0, 0, 0, 0.3);
        cursor: pointer;
        transition: all .2s
    }

    #adblock button.active {
        background: #fff
    }

    #adblock .tutorial {
        background: #fff;
        text-align: left;
        color: #000;
        padding: 20px;
        height: 250px;
        overflow: auto;
        line-height: 30px
    }

    #adblock .tutorial div {
        display: none
    }

    #adblock .tutorial div.active {
        display: block
    }

    #adblock ol {
        margin-left: 20px
    }

    @media(max-width:680px) {
        #adblock .inner {
            width: calc(100% - 80px);
            margin: auto
        }
    }
</style>
```
5. Add below code at the end of your theme i.e before closing of </body> tag

```
<script src='https://cdn.jsdelivr.net/gh/RockBlogger/Anti-AdBlocker@main/2.0/code.min.js'/>
```

6. Click on Save the Theme

7. Now Refresh your Website. It will looks like as below image

![adblocker](https://user-images.githubusercontent.com/26889268/223098820-55a6f305-0979-4ba5-a8a9-789d236b7a67.png)
