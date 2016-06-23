# simplejsbox
Dit JavaScript framework is voor mensen die nog totaal geen ervaring hebben met JavaScript en zo de simpelste functies makkelijk leren gebruiken.

In gebruik:

1. Voeg <script src="js/simplejsbox.js"></script> toe in de <head> van je code.
2. Voeg de volgende code toe tussen je <body></body> tags om de 'box' zichtbaar te maken en de JavaScript werkend te krijgen.                 <style>
        input[type=text] {
            font-size: 20px;
        }
        </style>
        <div style="margin:10px; padding:30px; border:1px solid #666; width:550px;">
                Dit is een demo voor een JavaScript framework, gemaakt door Timo Bergmans.<br><br>
                De simpelste functies van JavaScript staan hier bij elkaar zodat je deze makkelijk leert begrijpen.
                <br><br>
                <input id="button" type="button" value="Change" onclick="btnTransform('Changed Text')">
                <input id="button3" type="button" value="Error" onclick="btnError('Error')">
                <input id="button1" type="button" value="Hide" onclick="btnHide()">
                <input id="button2" type="button" value="Show" onclick="btnShow()">
                <input id="button4" type="button" value="Rood" onclick="btnBgColor('#ff0000')">
                <input id="button5" type="button" value="Wit" onclick="btnBgColor('#ffffff')">
                <input id="button5" type="button" value="Blauw" onclick="btnBgColor('#3477B4')">                
                <input id="button6" type="button" value="Toggle" onclick="toggle();">
                <input id="button8" type="button" value="Event Chaining" onclick="chain();">
                <br>
                <input id="text" type="text" value="default" style="margin:50px">
                <script type="text/javascript">
                    function btnTransform(newValue) {
                        _('text').val(newValue);
                        var obj = new _('text');
                        obj.val("Deze tekst kan veranderen");
                    }
                    function btnError(newValue) {
                        _('text').val(newValue).bgcolor('#dddddd');
                    }
                    function btnHide() {
                        _('text').hide();
                    }
                    function btnShow() {
                        _('text').show();
                    }
                    function btnBgColor(color) {
                        _('text').bgcolor(color);
                    }
                    function toggle() {
                        _('text').toggle();
                    }
                    function chain() {
                        _('text').size(200, 440).bgcolor('#3477B4');
                    }                 
                </script>
        </div> 

Motivatie:

Ik heb het coderen met JavaScript zelf al best wel onder de knie, maar ik hoor vaak van mensen dat zij JavaScript of jQuery ontwijken omdat ze er nog nooit mee hebben gewerkt. Daarom heb ik deze simpele 'SimpleJS Box' gemaakt zodat mensen rustig kunnen bekijken hoe een aantal simpele JavaScript functies werken en hoe deze worden geschreven in code.

Gemaakt door Timo Bergmans.
