# Github Flavored Markdown Syntax #
_The unofficial cheat sheet for the **.md** files_
------

GitHub uses its own unique render to display **.md** files in your Internet Browser of choice. Commonly known as "GitHub Flavored Markdown," or GFM, it is used across the system to render **.md** files (A.K.A. "_documents_"), which are used in wiki pages, project documents, issues tracking, comments, and pull requests. 

The GFM rendering process differs from Standard Markdown (SM) in a few significant ways. It also adds few key functionalities and adjust the render tailoring it for Github usage purposes. You can lear more about it at <a href="https://github.com/github/markup#markups" target="_blank">Github Markups</a>. 

If you're not already familiar with **Markdown**, take a look at some **Markdown Basics** (<a href="https://www.google.com/#newwindow=1&safe=off&q=%22Markdown+Basics%22+tutorials" target="_blank">search for it on Google</a>), there are great tutorials available). Just remember Github's GFM has extra features that are tailored for its own needs, such as: pull request integration, SHA-1 Conversion (see below), task lists and more.

An important remark for anyone writing documentation inside Github projects: the GFM render recognizes **HTML TAGS** and render them properly, but not aggressively sanitize the HTML, such as: script tags, (some) inline-styles, and classes or id attributes. See the <a href="https://github.com/rgrove/sanitize/#readme" target="_blank">sanitization filter</a> for the full whitelisted HTML list. So, few free to use Markup, HTML Tags or both at same time. Try it and see for yourself. Sure enought you will find situations in which HTML TAGS will better fit than the equivalent Markdown and vice-versa.

Express your freedom and have a great writting experience.

## Text Formatting Markdown ##

<table width="100%" valign="top" style='border: none;'>
<thead>
<tr>
  <td width="20%" nowrap>Markdown</td>
  <td width="20%" nowrap>Will Render As</td>
  <td width="0%">Notes & References</td>
</tr>
</thead>
<tbody>
<tr>
  <td width="20%" valign="top" nowrap><code># Heading 1 #</code></td>
  <td width="20%" valign="top" nowrap><h1>Heading 1</h1></td>
  <td width="0%" valign="top">
      Equivalent to <code><b>&lt;h1&gt;</b></code> tag, but with a thin <i>horizontal underline</i> attached.<br /><br />
      Same effect can be obtained by adding <code>===</code> as the very next paragraph.
  </td>
</tr>
<tr>
  <td width="20%" valign="top" nowrap><code>## Heading 2 ##</code></td>
  <td width="20%" valign="top" nowrap><h2>Heading 2</h2></td>
  <td width="0%" valign="top">
      Equivalent to <code><b>&lt;h2&gt;</b></code> tag, but with a thin <i>horizontal underline</i> attached.<br /><br />
      Same effect can be obtained by adding <code>---</code> as the very next paragraph.
  </td>
</tr>
<tr>
  <td width="20%" valign="top" nowrap><code>### Heading 3 ###</code></td>
  <td width="20%" valign="top" nowrap><h3>Heading 3</h3></td>
  <td width="0%" valign="top">Equivalent to <code><b>&lt;h3&gt;</b></code> tag.</td>
</tr>
<tr>
  <td width="20%" valign="top" nowrap><code>#### Heading 4 ####</code></td>
  <td width="20%" valign="top" nowrap><h4>Heading 4</h4></td>
  <td width="0%" valign="top">Equivalent to <code><b>&lt;h4&gt;</b></code> tag.</td>
</tr>
<tr>
  <td width="20%" valign="top" nowrap><code>##### Heading 5 #####</code></td>
  <td width="20%" valign="top" nowrap><h5>Heading 5</h5></td>
  <td width="0%" valign="top">Equivalent to <code><b>&lt;h5&gt;</b></code> tag.</td>
</tr>
<tr>
  <td width="20%" valign="top" nowrap><code>###### Heading 6 ######</code></td>
  <td width="20%" valign="top" nowrap><h6>Heading 6</h6></td>
  <td width="0%" valign="top">Equivalent to <code><b>&lt;h6&gt;</b></code> tag.</td>
</tr>
</tbody>
</table>


Notes:
Available Languages for the language block: https://github.com/github/linguist/blob/master/lib/linguist/languages.yml

Emoji Unicode Table:
http://apps.timwhitlock.info/emoji/tables/unicode
&#x2702

	
In case this may be helpful for someone who just needs to show colors rather than output, as a hackish workaround (and FYI), since Github supports Unicode numeric character references (and HTML entities), you could try colored Unicode symbols, though it depends on the font rendering them in color (as it happens to be appearing for me on Windows 10 at least):

* RED APPLE (&#x1F34E;): 🍎
* GREEN APPLE (&#x1F34F;): 🍏
* BLUE HEART (&#x1F499;): 💙
* GREEN HEART (&#x1F49A;): 💚
* YELLOW HEART (&#x1F49B;): 💛
* PURPLE HEART (&#x1F49C;): 💜
* GREEN BOOK (&#x1F4D7;): 📗
* BLUE BOOK (&#x1F4D8;): 📘
* ORANGE BOOK (&#x1F4D9;): 📙
* LARGE RED CIRCLE (&#x1F534;): 🔴
* LARGE BLUE CIRCLE (&#x1F535;): 🔵
* LARGE ORANGE DIAMOND (&#x1F536;): 🔶
* LARGE BLUE DIAMOND (&#x1F537;): 🔷
* SMALL ORANGE DIAMOND (&#x1F538;): 🔸
* SMALL BLUE DIAMOND (&#x1F539;): 🔹
* UP-POINTING RED TRIANGLE (&#x1F53A;): 🔺
* DOWN-POINTING RED TRIANGLE (&#x1F53B;): 🔻
* UP-POINTING SMALL RED TRIANGLE (&#x1F53C;): 🔼
* DOWN-POINTING SMALL RED TRIANGLE (&#x1F53D;): 🔽
* 

©️ Copyright Sign
®️ Registered Sign
‼️ Double Exclamation Mark
⁉️ Exclamation Question Mark
™️ Trade Mark Sign
ℹ️ Information Source
↔️ Left Right Arrow
↕️ Up Down Arrow
↖️ North West Arrow
↗️ North East Arrow
↘️ South East Arrow
↙️ South West Arrow
↩️ Leftwards Arrow With Hook
↪️ Rightwards Arrow With Hook
⌚ Watch
⌛ Hourglass
⌨ Keyboard
⏏ Eject Symbol
⏩ Black Right-Pointing Double Triangle
⏪ Black Left-Pointing Double Triangle
⏫ Black Up-Pointing Double Triangle
⏬ Black Down-Pointing Double Triangle
⏭ Black Right-Pointing Double Triangle With Vertical Bar
⏮ Black Left-Pointing Double Triangle With Vertical Bar
⏯ Black Right-Pointing Triangle With Double Vertical Bar
⏰ Alarm Clock
⏱ Stopwatch
⏲ Timer Clock
⏳ Hourglass With Flowing Sand
⏸ Double Vertical Bar
⏹ Black Square for Stop
⏺ Black Circle for Record
▪️ Black Small Square
▫️ White Small Square
▶️ Black Right-Pointing Triangle
◀️ Black Left-Pointing Triangle
◻️ White Medium Square
◼️ Black Medium Square
◽ White Medium Small Square
◾ Black Medium Small Square
☀️ Black Sun With Rays
☁️ Cloud
☂ Umbrella
☃ Snowman
☄ Comet
☎️ Black Telephone
☑️ Ballot Box With Check
☔ Umbrella With Rain Drops
☕ Hot Beverage
☘ Shamrock
☝️ White Up Pointing Index
☠ Skull and Crossbones
☢ Radioactive Sign
☣ Biohazard Sign
☦ Orthodox Cross
☪ Star and Crescent
☮ Peace Symbol
☯ Yin Yang
☸ Wheel of Dharma
☹ White Frowning Face
☺️ White Smiling Face
♈ Aries
♉ Taurus
♊ Gemini
♋ Cancer
♌ Leo
♍ Virgo
♎ Libra
♏ Scorpius
♐ Sagittarius
♑ Capricorn
♒ Aquarius
♓ Pisces
♠️ Black Spade Suit
♣️ Black Club Suit
♥️ Black Heart Suit
♦️ Black Diamond Suit
♨️ Hot Springs
♻️ Black Universal Recycling Symbol
♿ Wheelchair Symbol
⚒ Hammer and Pick
⚓ Anchor
⚔ Crossed Swords
⚖ Scales
⚗ Alembic
⚙ Gear
⚛ Atom Symbol
⚜ Fleur-De-Lis
⚠️ Warning Sign
⚡ High Voltage Sign
⚪ Medium White Circle
⚫ Medium Black Circle
⚰ Coffin
⚱ Funeral Urn
⚽ Soccer Ball
⚾ Baseball
⛄ Snowman Without Snow
⛅ Sun Behind Cloud
⛈ Thunder Cloud and Rain
⛎ Ophiuchus
⛏ Pick
⛑ Helmet With White Cross
⛓ Chains
⛔ No Entry
⛩ Shinto Shrine
⛪ Church
⛰ Mountain
⛱ Umbrella on Ground
⛲ Fountain
⛳ Flag in Hole
⛴ Ferry
⛵ Sailboat
⛷ Skier
⛸ Ice Skate
⛹ Person With Ball
⛺ Tent
⛽ Fuel Pump
✂️ Black Scissors
✅ White Heavy Check Mark
✈️ Airplane
✉️ Envelope
✊ Raised Fist
✋ Raised Hand
✌️ Victory Hand
✍ Writing Hand
✏️ Pencil
✒️ Black Nib
✔️ Heavy Check Mark
✖️ Heavy Multiplication X
✝ Latin Cross
✡ Star of David
✨ Sparkles
✳️ Eight Spoked Asterisk
✴️ Eight Pointed Black Star
❄️ Snowflake
❇️ Sparkle
❌ Cross Mark
❎ Negative Squared Cross Mark
❓ Black Question Mark Ornament
❔ White Question Mark Ornament
❕ White Exclamation Mark Ornament
❗ Heavy Exclamation Mark Symbol
❣ Heavy Heart Exclamation Mark Ornament
❤️ Heavy Black Heart
➕ Heavy Plus Sign
➖ Heavy Minus Sign
➗ Heavy Division Sign
➡️ Black Rightwards Arrow
➰ Curly Loop
➿ Double Curly Loop
⤴️ Arrow Pointing Rightwards Then Curving Upwards
⤵️ Arrow Pointing Rightwards Then Curving Downwards
⬅️ Leftwards Black Arrow
⬆️ Upwards Black Arrow
⬇️ Downwards Black Arrow
⬛ Black Large Square
⬜ White Large Square
⭐ White Medium Star
⭕ Heavy Large Circle
🀄 Mahjong Tile Red Dragon
🃏 Playing Card Black Joker
🅰️ Negative Squared Latin Capital Letter A
🅱️ Negative Squared Latin Capital Letter B
🅾️ Negative Squared Latin Capital Letter O
🅿️ Negative Squared Latin Capital Letter P
🆎 Negative Squared AB
🆑 Squared CL
🆒 Squared Cool
🆓 Squared Free
🆔 Squared ID
🆕 Squared New
🆖 Squared NG
🆗 Squared OK
🆘 Squared SOS
🆙 Squared Up With Exclamation Mark
🆚 Squared Vs
🈁 Squared Katakana Koko
🈂️ Squared Katakana Sa
🈚 Squared CJK Unified Ideograph-7121
🈯 Squared CJK Unified Ideograph-6307
🈲 Squared CJK Unified Ideograph-7981
🈳 Squared CJK Unified Ideograph-7a7a
🈴 Squared CJK Unified Ideograph-5408
🈵 Squared CJK Unified Ideograph-6e80
🈶 Squared CJK Unified Ideograph-6709
🈷️ Squared CJK Unified Ideograph-6708
🈸 Squared CJK Unified Ideograph-7533
🈹 Squared CJK Unified Ideograph-5272
🈺 Squared CJK Unified Ideograph-55b6
🉐 Circled Ideograph Advantage
🉑 Circled Ideograph Accept
🌀 Cyclone
🌁 Foggy
🌂 Closed Umbrella
🌃 Night With Stars
🌄 Sunrise Over Mountains
🌅 Sunrise
🌆 Cityscape at Dusk
🌇 Sunset Over Buildings
🌈 Rainbow
🌉 Bridge at Night
🌊 Water Wave
🌋 Volcano
🌌 Milky Way
🌍 Earth Globe Europe-Africa
🌎 Earth Globe Americas
🌏 Earth Globe Asia-Australia
🌐 Globe With Meridians
🌑 New Moon Symbol
🌒 Waxing Crescent Moon Symbol
🌓 First Quarter Moon Symbol
🌔 Waxing Gibbous Moon Symbol
🌕 Full Moon Symbol
🌖 Waning Gibbous Moon Symbol
🌗 Last Quarter Moon Symbol
🌘 Waning Crescent Moon Symbol
🌙 Crescent Moon
🌚 New Moon With Face
🌛 First Quarter Moon With Face
🌜 Last Quarter Moon With Face
🌝 Full Moon With Face
🌞 Sun With Face
🌟 Glowing Star
🌠 Shooting Star
🌡 Thermometer
🌤 White Sun With Small Cloud
🌥 White Sun Behind Cloud
🌦 White Sun Behind Cloud With Rain
🌧 Cloud With Rain
🌨 Cloud With Snow
🌩 Cloud With Lightning
🌪 Cloud With Tornado
🌫 Fog
🌬 Wind Blowing Face
🌭 Hot Dog
🌮 Taco
🌯 Burrito
🌰 Chestnut
🌱 Seedling
🌲 Evergreen Tree
🌳 Deciduous Tree
🌴 Palm Tree
🌵 Cactus
🌶 Hot Pepper
🌷 Tulip
🌸 Cherry Blossom
🌹 Rose
🌺 Hibiscus
🌻 Sunflower
🌼 Blossom
🌽 Ear of Maize
🌾 Ear of Rice
🌿 Herb
🍀 Four Leaf Clover
🍁 Maple Leaf
🍂 Fallen Leaf
🍃 Leaf Fluttering in Wind
🍄 Mushroom
🍅 Tomato
🍆 Aubergine
🍇 Grapes
🍈 Melon
🍉 Watermelon
🍊 Tangerine
🍋 Lemon
🍌 Banana
🍍 Pineapple
🍎 Red Apple
🍏 Green Apple
🍐 Pear
🍑 Peach
🍒 Cherries
🍓 Strawberry
🍔 Hamburger
🍕 Slice of Pizza
🍖 Meat on Bone
🍗 Poultry Leg
🍘 Rice Cracker
🍙 Rice Ball
🍚 Cooked Rice
🍛 Curry and Rice
🍜 Steaming Bowl
🍝 Spaghetti
🍞 Bread
🍟 French Fries
🍠 Roasted Sweet Potato
🍡 Dango
🍢 Oden
🍣 Sushi
🍤 Fried Shrimp
🍥 Fish Cake With Swirl Design
🍦 Soft Ice Cream
🍧 Shaved Ice
🍨 Ice Cream
🍩 Doughnut
🍪 Cookie
🍫 Chocolate Bar
🍬 Candy
🍭 Lollipop
🍮 Custard
🍯 Honey Pot
🍰 Shortcake
🍱 Bento Box
🍲 Pot of Food
🍳 Cooking
🍴 Fork and Knife
🍵 Teacup Without Handle
🍶 Sake Bottle and Cup
🍷 Wine Glass
🍸 Cocktail Glass
🍹 Tropical Drink
🍺 Beer Mug
🍻 Clinking Beer Mugs
🍼 Baby Bottle
🍽 Fork and Knife With Plate
🍾 Bottle With Popping Cork
🍿 Popcorn
🎀 Ribbon
🎁 Wrapped Present
🎂 Birthday Cake
🎃 Jack-O-Lantern
🎄 Christmas Tree
🎅 Father Christmas
🎆 Fireworks
🎇 Firework Sparkler
🎈 Balloon
🎉 Party Popper
🎊 Confetti Ball
🎋 Tanabata Tree
🎌 Crossed Flags
🎍 Pine Decoration
🎎 Japanese Dolls
🎏 Carp Streamer
🎐 Wind Chime
🎑 Moon Viewing Ceremony
🎒 School Satchel
🎓 Graduation Cap
🎖 Military Medal
🎗 Reminder Ribbon
🎙 Studio Microphone
🎚 Level Slider
🎛 Control Knobs
🎞 Film Frames
🎟 Admission Tickets
🎠 Carousel Horse
🎡 Ferris Wheel
🎢 Roller Coaster
🎣 Fishing Pole and Fish
🎤 Microphone
🎥 Movie Camera
🎦 Cinema
🎧 Headphone
🎨 Artist Palette
🎩 Top Hat
🎪 Circus Tent
🎫 Ticket
🎬 Clapper Board
🎭 Performing Arts
🎮 Video Game
🎯 Direct Hit
🎰 Slot Machine
🎱 Billiards
🎲 Game Die
🎳 Bowling
🎴 Flower Playing Cards
🎵 Musical Note
🎶 Multiple Musical Notes
🎷 Saxophone
🎸 Guitar
🎹 Musical Keyboard
🎺 Trumpet
🎻 Violin
🎼 Musical Score
🎽 Running Shirt With Sash
🎾 Tennis Racquet and Ball
🎿 Ski and Ski Boot
🏀 Basketball and Hoop
🏁 Chequered Flag
🏂 Snowboarder
🏃 Runner
🏄 Surfer
🏅 Sports Medal
🏆 Trophy
🏇 Horse Racing
🏈 American Football
🏉 Rugby Football
🏊 Swimmer
🏋 Weight Lifter
🏌 Golfer
🏍 Racing Motorcycle
🏎 Racing Car
🏏 Cricket Bat and Ball
🏐 Volleyball
🏑 Field Hockey Stick and Ball
🏒 Ice Hockey Stick and Puck
🏓 Table Tennis Paddle and Ball
🏔 Snow Capped Mountain
🏕 Camping
🏖 Beach With Umbrella
🏗 Building Construction
🏘 House Buildings
🏙 Cityscape
🏚 Derelict House Building
🏛 Classical Building
🏜 Desert
🏝 Desert Island
🏞 National Park
🏟 Stadium
🏠 House Building
🏡 House With Garden
🏢 Office Building
🏣 Japanese Post Office
🏤 European Post Office
🏥 Hospital
🏦 Bank
🏧 Automated Teller Machine
🏨 Hotel
🏩 Love Hotel
🏪 Convenience Store
🏫 School
🏬 Department Store
🏭 Factory
🏮 Izakaya Lantern
🏯 Japanese Castle
🏰 European Castle
🏳 Waving White Flag
🏴 Waving Black Flag
🏵 Rosette
🏷 Label
🏸 Badminton Racquet and Shuttlecock
🏹 Bow and Arrow
🏺 Amphora
🐀 Rat
🐁 Mouse
🐂 Ox
🐃 Water Buffalo
🐄 Cow
🐅 Tiger
🐆 Leopard
🐇 Rabbit
🐈 Cat
🐉 Dragon
🐊 Crocodile
🐋 Whale
🐌 Snail
🐍 Snake
🐎 Horse
🐏 Ram
🐐 Goat
🐑 Sheep
🐒 Monkey
🐓 Rooster
🐔 Chicken
🐕 Dog
🐖 Pig
🐗 Boar
🐘 Elephant
🐙 Octopus
🐚 Spiral Shell
🐛 Bug
🐜 Ant
🐝 Honeybee
🐞 Lady Beetle
🐟 Fish
🐠 Tropical Fish
🐡 Blowfish
🐢 Turtle
🐣 Hatching Chick
🐤 Baby Chick
🐥 Front-Facing Baby Chick
🐦 Bird
🐧 Penguin
🐨 Koala
🐩 Poodle
🐪 Dromedary Camel
🐫 Bactrian Camel
🐬 Dolphin
🐭 Mouse Face
🐮 Cow Face
🐯 Tiger Face
🐰 Rabbit Face
🐱 Cat Face
🐲 Dragon Face
🐳 Spouting Whale
🐴 Horse Face
🐵 Monkey Face
🐶 Dog Face
🐷 Pig Face
🐸 Frog Face
🐹 Hamster Face
🐺 Wolf Face
🐻 Bear Face
🐼 Panda Face
🐽 Pig Nose
🐾 Paw Prints
🐿 Chipmunk
👀 Eyes
👁 Eye
👂 Ear
👃 Nose
👄 Mouth
👅 Tongue
👆 White Up Pointing Backhand Index
👇 White Down Pointing Backhand Index
👈 White Left Pointing Backhand Index
👉 White Right Pointing Backhand Index
👊 Fisted Hand Sign
👋 Waving Hand Sign
👌 OK Hand Sign
👍 Thumbs Up Sign
👎 Thumbs Down Sign
👏 Clapping Hands Sign
👐 Open Hands Sign
👑 Crown
👒 Womans Hat
👓 Eyeglasses
👔 Necktie
👕 T-Shirt
👖 Jeans
👗 Dress
👘 Kimono
👙 Bikini
👚 Womans Clothes
👛 Purse
👜 Handbag
👝 Pouch
👞 Mans Shoe
👟 Athletic Shoe
👠 High-Heeled Shoe
👡 Womans Sandal
👢 Womans Boots
👣 Footprints
👤 Bust in Silhouette
👥 Busts in Silhouette
👦 Boy
👧 Girl
👨 Man
👩 Woman
👪 Family
👫 Man and Woman Holding Hands
👬 Two Men Holding Hands
👭 Two Women Holding Hands
👮 Police Officer
👯 Woman With Bunny Ears
👰 Bride With Veil
👱 Person With Blond Hair
👲 Man With Gua Pi Mao
👳 Man With Turban
👴 Older Man
👵 Older Woman
👶 Baby
👷 Construction Worker
👸 Princess
👹 Japanese Ogre
👺 Japanese Goblin
👻 Ghost
👼 Baby Angel
👽 Extraterrestrial Alien
👾 Alien Monster
👿 Imp
💀 Skull
💁 Information Desk Person
💂 Guardsman
💃 Dancer
💄 Lipstick
💅 Nail Polish
💆 Face Massage
💇 Haircut
💈 Barber Pole
💉 Syringe
💊 Pill
💋 Kiss Mark
💌 Love Letter
💍 Ring
💎 Gem Stone
💏 Kiss
💐 Bouquet
💑 Couple With Heart
💒 Wedding
💓 Beating Heart
💔 Broken Heart
💕 Two Hearts
💖 Sparkling Heart
💗 Growing Heart
💘 Heart With Arrow
💙 Blue Heart
💚 Green Heart
💛 Yellow Heart
💜 Purple Heart
💝 Heart With Ribbon
💞 Revolving Hearts
💟 Heart Decoration
💠 Diamond Shape With a Dot Inside
💡 Electric Light Bulb
💢 Anger Symbol
💣 Bomb
💤 Sleeping Symbol
💥 Collision Symbol
💦 Splashing Sweat Symbol
💧 Droplet
💨 Dash Symbol
💩 Pile of Poo
💪 Flexed Biceps
💫 Dizzy Symbol
💬 Speech Balloon
💭 Thought Balloon
💮 White Flower
💯 Hundred Points Symbol
💰 Money Bag
💱 Currency Exchange
💲 Heavy Dollar Sign
💳 Credit Card
💴 Banknote With Yen Sign
💵 Banknote With Dollar Sign
💶 Banknote With Euro Sign
💷 Banknote With Pound Sign
💸 Money With Wings
💹 Chart With Upwards Trend and Yen Sign
💺 Seat
💻 Personal Computer
💼 Briefcase
💽 Minidisc
💾 Floppy Disk
💿 Optical Disc
📀 DVD
📁 File Folder
📂 Open File Folder
📃 Page With Curl
📄 Page Facing Up
📅 Calendar
📆 Tear-Off Calendar
📇 Card Index
📈 Chart With Upwards Trend
📉 Chart With Downwards Trend
📊 Bar Chart
📋 Clipboard
📌 Pushpin
📍 Round Pushpin
📎 Paperclip
📏 Straight Ruler
📐 Triangular Ruler
📑 Bookmark Tabs
📒 Ledger
📓 Notebook
📔 Notebook With Decorative Cover
📕 Closed Book
📖 Open Book
📗 Green Book
📘 Blue Book
📙 Orange Book
📚 Books
📛 Name Badge
📜 Scroll
📝 Memo
📞 Telephone Receiver
📟 Pager
📠 Fax Machine
📡 Satellite Antenna
📢 Public Address Loudspeaker
📣 Cheering Megaphone
📤 Outbox Tray
📥 Inbox Tray
📦 Package
📧 E-Mail Symbol
📨 Incoming Envelope
📩 Envelope With Downwards Arrow Above
📪 Closed Mailbox With Lowered Flag
📫 Closed Mailbox With Raised Flag
📬 Open Mailbox With Raised Flag
📭 Open Mailbox With Lowered Flag
📮 Postbox
📯 Postal Horn
📰 Newspaper
📱 Mobile Phone
📲 Mobile Phone With Rightwards Arrow at Left
📳 Vibration Mode
📴 Mobile Phone Off
📵 No Mobile Phones
📶 Antenna With Bars
📷 Camera
📸 Camera With Flash
📹 Video Camera
📺 Television
📻 Radio
📼 Videocassette
📽 Film Projector
📿 Prayer Beads
🔀 Twisted Rightwards Arrows
🔁 Clockwise Rightwards and Leftwards Open Circle Arrows
🔂 Clockwise Rightwards and Leftwards Open Circle Arrows With Circled One Overlay
🔃 Clockwise Downwards and Upwards Open Circle Arrows
🔄 Anticlockwise Downwards and Upwards Open Circle Arrows
🔅 Low Brightness Symbol
🔆 High Brightness Symbol
🔇 Speaker With Cancellation Stroke
🔈 Speaker
🔉 Speaker With One Sound Wave
🔊 Speaker With Three Sound Waves
🔋 Battery
🔌 Electric Plug
🔍 Left-Pointing Magnifying Glass
🔎 Right-Pointing Magnifying Glass
🔏 Lock With Ink Pen
🔐 Closed Lock With Key
🔑 Key
🔒 Lock
🔓 Open Lock
🔔 Bell
🔕 Bell With Cancellation Stroke
🔖 Bookmark
🔗 Link Symbol
🔘 Radio Button
🔙 Back With Leftwards Arrow Above
🔚 End With Leftwards Arrow Above
🔛 On With Exclamation Mark With Left Right Arrow Above
🔜 Soon With Rightwards Arrow Above
🔝 Top With Upwards Arrow Above
🔞 No One Under Eighteen Symbol
🔟 Keycap Ten
🔠 Input Symbol for Latin Capital Letters
🔡 Input Symbol for Latin Small Letters
🔢 Input Symbol for Numbers
🔣 Input Symbol for Symbols
🔤 Input Symbol for Latin Letters
🔥 Fire
🔦 Electric Torch
🔧 Wrench
🔨 Hammer
🔩 Nut and Bolt
🔪 Hocho
🔫 Pistol
🔬 Microscope
🔭 Telescope
🔮 Crystal Ball
🔯 Six Pointed Star With Middle Dot
🔰 Japanese Symbol for Beginner
🔱 Trident Emblem
🔲 Black Square Button
🔳 White Square Button
🔴 Large Red Circle
🔵 Large Blue Circle
🔶 Large Orange Diamond
🔷 Large Blue Diamond
🔸 Small Orange Diamond
🔹 Small Blue Diamond
🔺 Up-Pointing Red Triangle
🔻 Down-Pointing Red Triangle
🔼 Up-Pointing Small Red Triangle
🔽 Down-Pointing Small Red Triangle
🕉 Om Symbol
🕊 Dove of Peace
🕋 Kaaba
🕌 Mosque
🕍 Synagogue
🕎 Menorah With Nine Branches
🕐 Clock Face One O'Clock
🕑 Clock Face Two O'Clock
🕒 Clock Face Three O'Clock
🕓 Clock Face Four O'Clock
🕔 Clock Face Five O'Clock
🕕 Clock Face Six O'Clock
🕖 Clock Face Seven O'Clock
🕗 Clock Face Eight O'Clock
🕘 Clock Face Nine O'Clock
🕙 Clock Face Ten O'Clock
🕚 Clock Face Eleven O'Clock
🕛 Clock Face Twelve O'Clock
🕜 Clock Face One-Thirty
🕝 Clock Face Two-Thirty
🕞 Clock Face Three-Thirty
🕟 Clock Face Four-Thirty
🕠 Clock Face Five-Thirty
🕡 Clock Face Six-Thirty
🕢 Clock Face Seven-Thirty
🕣 Clock Face Eight-Thirty
🕤 Clock Face Nine-Thirty
🕥 Clock Face Ten-Thirty
🕦 Clock Face Eleven-Thirty
🕧 Clock Face Twelve-Thirty
🕯 Candle
🕰 Mantelpiece Clock
🕳 Hole
🕴 Man in Business Suit Levitating
🕵 Sleuth or Spy
🕶 Dark Sunglasses
🕷 Spider
🕸 Spider Web
🕹 Joystick
🕺 Man Dancing
🖇 Linked Paperclips
🖊 Lower Left Ballpoint Pen
🖋 Lower Left Fountain Pen
🖌 Lower Left Paintbrush
🖍 Lower Left Crayon
🖐 Raised Hand With Fingers Splayed
🖕 Reversed Hand With Middle Finger Extended
🖖 Raised Hand With Part Between Middle and Ring Fingers
🖤 Black Heart
🖥 Desktop Computer
🖨 Printer
🖱 Three Button Mouse
🖲 Trackball
🖼 Frame With Picture
🗂 Card Index Dividers
🗃 Card File Box
🗄 File Cabinet
🗑 Wastebasket
🗒 Spiral Note Pad
🗓 Spiral Calendar Pad
🗜 Compression
🗝 Old Key
🗞 Rolled-Up Newspaper
🗡 Dagger Knife
🗣 Speaking Head in Silhouette
🗨 Left Speech Bubble
🗯 Right Anger Bubble
🗳 Ballot Box With Ballot
🗺 World Map
🗻 Mount Fuji
🗼 Tokyo Tower
🗽 Statue of Liberty
🗾 Silhouette of Japan
🗿 Moyai
😀 Grinning Face
😁 Grinning Face With Smiling Eyes
😂 Face With Tears of Joy
😃 Smiling Face With Open Mouth
😄 Smiling Face With Open Mouth and Smiling Eyes
😅 Smiling Face With Open Mouth and Cold Sweat
😆 Smiling Face With Open Mouth and Tightly-Closed Eyes
😇 Smiling Face With Halo
😈 Smiling Face With Horns
😉 Winking Face
😊 Smiling Face With Smiling Eyes
😋 Face Savouring Delicious Food
😌 Relieved Face
😍 Smiling Face With Heart-Shaped Eyes
😎 Smiling Face With Sunglasses
😏 Smirking Face
😐 Neutral Face
😑 Expressionless Face
😒 Unamused Face
😓 Face With Cold Sweat
😔 Pensive Face
😕 Confused Face
😖 Confounded Face
😗 Kissing Face
😘 Face Throwing a Kiss
😙 Kissing Face With Smiling Eyes
😚 Kissing Face With Closed Eyes
😛 Face With Stuck-Out Tongue
😜 Face With Stuck-Out Tongue and Winking Eye
😝 Face With Stuck-Out Tongue and Tightly-Closed Eyes
😞 Disappointed Face
😟 Worried Face
😠 Angry Face
😡 Pouting Face
😢 Crying Face
😣 Persevering Face
😤 Face With Look of Triumph
😥 Disappointed but Relieved Face
😦 Frowning Face With Open Mouth
😧 Anguished Face
😨 Fearful Face
😩 Weary Face
😪 Sleepy Face
😫 Tired Face
😬 Grimacing Face
😭 Loudly Crying Face
😮 Face With Open Mouth
😯 Hushed Face
😰 Face With Open Mouth and Cold Sweat
😱 Face Screaming in Fear
😲 Astonished Face
😳 Flushed Face
😴 Sleeping Face
😵 Dizzy Face
😶 Face Without Mouth
😷 Face With Medical Mask
😸 Grinning Cat Face With Smiling Eyes
😹 Cat Face With Tears of Joy
😺 Smiling Cat Face With Open Mouth
😻 Smiling Cat Face With Heart-Shaped Eyes
😼 Cat Face With Wry Smile
😽 Kissing Cat Face With Closed Eyes
😾 Pouting Cat Face
😿 Crying Cat Face
🙀 Weary Cat Face
🙁 Slightly Frowning Face
🙂 Slightly Smiling Face
🙃 Upside-Down Face
🙄 Face With Rolling Eyes
🙅 Face With No Good Gesture
🙆 Face With OK Gesture
🙇 Person Bowing Deeply
🙈 See-No-Evil Monkey
🙉 Hear-No-Evil Monkey
🙊 Speak-No-Evil Monkey
🙋 Happy Person Raising One Hand
🙌 Person Raising Both Hands in Celebration
🙍 Person Frowning
🙎 Person With Pouting Face
🙏 Person With Folded Hands
🚀 Rocket
🚁 Helicopter
🚂 Steam Locomotive
🚃 Railway Car
🚄 High-Speed Train
🚅 High-Speed Train With Bullet Nose
🚆 Train
🚇 Metro
🚈 Light Rail
🚉 Station
🚊 Tram
🚋 Tram Car
🚌 Bus
🚍 Oncoming Bus
🚎 Trolleybus
🚏 Bus Stop
🚐 Minibus
🚑 Ambulance
🚒 Fire Engine
🚓 Police Car
🚔 Oncoming Police Car
🚕 Taxi
🚖 Oncoming Taxi
🚗 Automobile
🚘 Oncoming Automobile
🚙 Recreational Vehicle
🚚 Delivery Truck
🚛 Articulated Lorry
🚜 Tractor
🚝 Monorail
🚞 Mountain Railway
🚟 Suspension Railway
🚠 Mountain Cableway
🚡 Aerial Tramway
🚢 Ship
🚣 Rowboat
🚤 Speedboat
🚥 Horizontal Traffic Light
🚦 Vertical Traffic Light
🚧 Construction Sign
🚨 Police Cars Revolving Light
🚩 Triangular Flag on Post
🚪 Door
🚫 No Entry Sign
🚬 Smoking Symbol
🚭 No Smoking Symbol
🚮 Put Litter in Its Place Symbol
🚯 Do Not Litter Symbol
🚰 Potable Water Symbol
🚱 Non-Potable Water Symbol
🚲 Bicycle
🚳 No Bicycles
🚴 Bicyclist
🚵 Mountain Bicyclist
🚶 Pedestrian
🚷 No Pedestrians
🚸 Children Crossing
🚹 Mens Symbol
🚺 Womens Symbol
🚻 Restroom
🚼 Baby Symbol
🚽 Toilet
🚾 Water Closet
🚿 Shower
🛀 Bath
🛁 Bathtub
🛂 Passport Control
🛃 Customs
🛄 Baggage Claim
🛅 Left Luggage
🛋 Couch and Lamp
🛌 Sleeping Accommodation
🛍 Shopping Bags
🛎 Bellhop Bell
🛏 Bed
🛐 Place of Worship
🛑 Octagonal Sign
🛒 Shopping Trolley
🛠 Hammer and Wrench
🛡 Shield
🛢 Oil Drum
🛣 Motorway
🛤 Railway Track
🛥 Motor Boat
🛩 Small Airplane
🛫 Airplane Departure
🛬 Airplane Arriving
🛰 Satellite
🛳 Passenger Ship
🛴 Scooter
🛵 Motor Scooter
🛶 Canoe
🤐 Zipper-Mouth Face
🤑 Money-Mouth Face
🤒 Face With Thermometer
🤓 Nerd Face
🤔 Thinking Face
🤕 Face With Head-Bandage
🤖 Robot Face
🤗 Hugging Face
🤘 Sign of the Horns
🤙 Call Me Hand
🤚 Raised Back Of Hand
🤛 Left-Facing Fist
🤜 Right-Facing Fist
🤝 Handshake
🤞 Hand With Index And Middle Fingers Crossed
🤠 Face With Cowboy Hat
🤡 Clown Face
🤢 Nauseated Face
🤣 Rolling On The Floor Laughing
🤤 Drooling Face
🤥 Lying Face
🤦 Face Palm
🤧 Sneezing Face
🤰 Pregnant Woman
🤳 Selfie
🤴 Prince
🤵 Man In Tuxedo
🤶 Mother Christmas
🤷 Shrug
🤸 Person Doing Cartwheel
🤹 Juggling
🤺 Fencer
🤼 Wrestlers
🤽 Water Polo
🤾 Handball
🥀 Wilted Flower
🥁 Drum With Drumsticks
🥂 Clinking Glasses
🥃 Tumbler Glass
🥄 Spoon
🥅 Goal Net
🥇 First Place Medal
🥈 Second Place Medal
🥉 Third Place Medal
🥊 Boxing Glove
🥋 Martial Arts Uniform
🥐 Croissant
🥑 Avocado
🥒 Cucumber
🥓 Bacon
🥔 Potato
🥕 Carrot
🥖 Baguette Bread
🥗 Green Salad
🥘 Shallow Pan Of Food
🥙 Stuffed Flatbread
🥚 Egg
🥛 Glass of Milk
🥜 Peanuts
🥝 Kiwifruit
🥞 Pancakes
🦀 Crab
🦁 Lion Face
🦂 Scorpion
🦃 Turkey
🦄 Unicorn Face
🦅 Eagle
🦆 Duck
🦇 Bat
🦈 Shark
🦉 Owl
🦊 Fox Face
🦋 Butterfly
🦌 Deer
🦍 Gorilla
🦎 Lizard
🦏 Rhinoceros
🦐 Shrimp
🦑 Squid
🧀 Cheese Wedge
