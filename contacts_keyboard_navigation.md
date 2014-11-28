# LinkedIn "Contacts" Keyboard Navigation

To enable "Contacts" section navigation with keyboard (instead of mouse-only) use the following javascript:

    javascript:
        /* Trigger on arrow keys */
        document.onkeyup = function(e) {
            e = e || window.event;

            /* Get button handlers */
            $next = $('button.next')[0];
            $prev = $('button.previous')[0];

            /* left -> prev*/
            if (e.keyCode == 37) {
                $prev.click();

            /* right -> next*/
            } else if (e.keyCode == 39) {
                $next.click();
            }
        };

## Chrome

Paste the above script to address bar. Double check that the "javascript:" prefix is present as Chrome strips it automatically as a protection mechanism.

## Firefox

Paste the above script to the developer console (ctrl + shift + c and select "console"). You will likely need to enter "allow paste" to the console as a security precaution.
