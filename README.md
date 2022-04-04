# Battery-Charging-Demo
Battery Charging Demo
<!DOCTYPE html>
<html lang="en">
<head>
    <style>
        @keyframes charging{
            100%{
                background-size: 120% 100%;
            }
        }
        .battry-charging{
            width: 160px;
            height: 80px;
            margin: 45px;
            border: 2px solid #3cb371;
            border-right-color: transparent;
            padding: 3px;
            background: repeating-linear-gradient(
                90deg,
                #3cb371 0 20px,
                #0000 0 30px
            )
            left/0% 100% no-repeat content-box
            content-box;
            position: relative;
            animation: charging 2s infinite steps(6);
        }
        .battry-charging::before{
            content: "";
            position: absolute;
            top: -2px;
            bottom: -2px;
            left: 100%;
            width: 10px;
            background: linear-gradient(
                #0000 calc(50% - 14px),
                #3cb371 0 calc(50% - 10px),
                #0000 0 calc(50% + 10px),
                #3cb371 0 calc(50% + 14px),
                #0000 0
            )
            left / 100% 100%,
            linear-gradient(
            #3cb371 calc(50% - 10px),
            #0000 0 calc(50% + 10px),
            #3cb371 0
            )
            left / 2px 100%,
            linear-gradient(
                #0000 calc(50% - 10px),
                #3cb371 0 calc(50% + 10px),
                #0000 0
            )
            right/4px 100%;
            background-repeat: no-repeat;
            
        }
    </style>
    <title>Battry Demo</title>
</head>
<body>
    <h1>Battry Charging Demo</h1>
    <div class="battry-charging"></div>
</body>
</html> 
