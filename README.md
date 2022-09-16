## Crypto Currency Mining Website Brief.
#### This is the landing page of a crypto currency mining platform called CRAPPO. It was created using React JS and AOS animation library.

#### To run:
````
npm create vite@latest my project
cd my-project

npm install
npm run dev
````
I have never created a landing page with as much content as this. However, I loved the flow from the introduction to the statistics to the valuation form down to the features section and the newsletter. It looked like something I would actually spend my time through. 

So, I got to work.

I glanced through the design file to understand how many sections there were. I created a react boilerplate with Vite and created each section as a component which I all added to a single page I named `Hero.jsx` .

I also created two button components; one with an icon and text as props and another with just a text passed as props. In case you're looking, they're named `Button.jsx` & `ButtonInfo.jsx`.

I made use of CSS  Flex and various flex properties for a good number of sections, especially those with more than one major content. Switching from `flex-direction: row` to `flex-direction: column` was the main trick behind the website's responsiveness. 

I inserted the various button components where necessary, because there were a lot of buttons!

The navigation was easy to pretty implement. For the mobile, I passed an `onClick` method to change state. Then, I implemented different stylings with the 2 states (true and false). So, when the hamburger was clicked, the state was toggled to 'true' and styling for the slide in menu was implemented. When toggled to 'false', the menu took on a styling to stay out of the DOM.

This same algorithm was applied to the individual cards that changed colour when clicked. However, I added  an extra function that toggled the state of the other cards to 'false' when one was 'true'.

My favourite part of the development was writing a  function to convert an inputed hashrate to an Ethereum value and then to a value in dollars. This can be found in the valution form in `Info.jsx`.

I did a bit of research on how hashrates affect mining and how they translated to blocks mined and implemented a conversion rate in the function. It worked out fine until I noticed that when the result was a continous decimal, the form outputed all the numbers and this distorted the UI of  the page.

So, I parsed the float value to 2 decimal places alone for both the ETH value and the dollar value.
Finally, I added the animations using the AOS library. I reduced the duration and delay for most elements for a smoother experience. 
Then, I created a repository on github and pushed the project. I used the github pages to host the site by running an npm run deploy on the terminal.

Danke!

Live  Site : https://ogoo-x.github.io/crypto-crappo/
