# 130. How to select breakpoints

Strategies for selecting breakpoints

## BAD Strategy: Based on popular devices

The problem with this strategy is that often new devices come in making it difficult for developer to maintain website applications ensuring their code works for those new devices.

## GOOD Strategy: Based on screen width range

Based on devices and ranges. Look at most used width for different categories of devices such as phones, tablet or desktop computers. Then group them together in some logical way to then pick out our breakpoints from that. This is better strategy than the first strategy as we not setting breakpoint at one specific device, but between similar device sizes such as smartphones, tablets - portrait, tablets - landscape, desktops (laptops).

Most smartphone screen size are between 300 - 500px and most tablets are 600 - 900px. Therefore, we can place a breakpoint at 600px. Same works for other categories.

Most landscape tablets are between 900px - 110px, most desktop are 1200px and over. Therefore, we can put a media querier at 1200px.

## Perfect Strategy: set breakpoint at places where the design breaks down

Forget about devices and only look at our content and our design.

We begin with one device either desktop or mobile size. Then we start decreasing our screen width or increasing it for mobile first. Then as soon as the design breaks (the design no longer looks acceptable), we create a new breakpoint. Try not to think about devices at all but its difficult to not to classify breakpoints as a phone, or a tablet etc. Therefore, we going to use this Perfect strategy with the Good strategy.
