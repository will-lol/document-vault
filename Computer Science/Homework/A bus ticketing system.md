# A bus ticketing system
A passenger can buy a single ticket as they get on the bus by paying with cash or with eftpos/credit/debit card. All the other forms of ticket can either be purchased from a physical store in the bus depot, or by ordering and paying online, after which the ticket will be sent to the customer in the mail.

## What are the usability problems with this system?
Usability issues with this particular system mainly come down to pleasant-ness and accessibility.
 - Sending bulk tickets in the mail may be expensive for the user
 - Sending bulk tickets in the mail is slow for the user
 - Users may not have a home or a place to mail tickets to
 - Making a trip to a physical location to buy tickets is inconvenient and slow
 - Making a trip to a physical location may be unfeasible for those with physical movement disabilities.
 - Physical tickets may get lost or damaged
 - For the vision impaired, hearing impaired buying a physical ticket may be more of an ordeal
 - Someone with a mental disability may struggle in terms of the overwhelming nature that going into town to buy a ticket provides or in other ways
 - The post system may deliver the tickets in such an untimely manner that they are no longer of use to the user

The bus company would like to upgrade its system and develop a virtual ticket that can be stored and displayed on a smart phone. The user can purchase any of the above ticket types using the app, and have a device on the bus verify the ticket. 

## What are the usability problems with this proposed system?

 - Some people may not have a phone to buy the ticket or to display it on
 - Some people may have a phone incompatible with the app
 - For those with vision disabilities, operating system level features may not apply to the app, or apply inconsistently or the app may not be designed with high contrast and visibility in mind
 - For those with mental disabilities, the app may not be well designed or not respect operating system level features
 - For those with physical disabilities, the app may not play well with hardware used to control the device
 - Being an app, it requires download and install which has an element of permanence. A user only using the app once may not require this
 - Being an app, the ticket may not integrate with the operating system level features (for example, Apple Pay or Google Pay transit features)

## How can we rectify some of these usability problems?

 - Most importantly, keep the offline parts of the legacy system around. Physical tickets still have merit for those without access to technology or with low technological literacy, which cannot be assumed in an area so ubiquitous as transport
 - Second most importantly, use a combination of technologies for authenticating the ticket. For users that support it, NFC could be used to make the authentication as easy as tapping onto the bus. The ticket could be integrated into the operating system using their respective wallet features. A QR code should be used on devices where NFC is not supported, so the ticket could be printed. The bus would need to be equipped with a device to read both of these formats, maybe an Android tablet?
 - Make it a web app. The browser makes it easy to integrate with operating system level accessibility features such as font size, reduced motion, high contrast and colour schemes. HTML and CSS are also easy to build in and reduce development costs, allowing more money to flow towards the design side of things. Web applications can also work offline using service workers and PWA technology, frequent users can install the app and use it as if it were native. Browsers are very ubiquitous and are great for adding cross platform. Users without a phone could feasibly use a library computer to make use of the system and print their digital tickets.