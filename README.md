# logiops-mxmaster3
My config for logiops


```
devices: (
{
    name: "Wireless Mouse MX Master 3";
    smartshift:
    {
        on: false;
        threshold: 30;
        torque: 50;
    };
    hiresscroll:
    {
        hires: true;
        invert: true;
        target: false;
    };
    dpi: 1200;

    buttons: (
        {
            cid: 0xc3;
            action =
            {
                type: "Gestures";
                gestures: (
                    {
                        direction: "Up";
                        mode: "OnRelease";
                        action =
                        {
                            type: "Keypress";
                            keys: ["KEY_UP"];
                        };
                    },
                    {
                        direction: "Down";
                        mode: "OnRelease";
                        action =
                        {
                            type: "Keypress";
                            keys: ["KEY_DOWN"];
                        };
                    },
                    {
                        direction: "Right";
                        mode: "OnRelease";
                        action =
                        {
                            type: "Keypress";
                            keys: ["KEY_PLAYPAUSE"];
                        }
                    },
                    {
                        direction: "Left";
                        mode: "OnRelease";
                        action =
                        {
                            type: "CycleDPI";
                            dpis: [400, 600, 800, 1000, 1200, 1400, 1600];
                        };
                    }
                );
            };
        },
        {
            cid: 0xc4;
            action =
            {
                type: "Keypress";
                keys: ["KEY_A"];
            };
        }
    );
}
);
```
