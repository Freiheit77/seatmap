# Jackson Hall_modify WC

This project aims to visualize the seatmap of a performing arts center. After using ovservable to map each and set up the x, y position for each seat, Tableau is used to do visualization. The sample outcome is like the following graph: 



https://observablehq.com/d/a821ebe900c694cc@128

View this notebook in your browser by running a web server in this folder. For
example:

~~~sh
python -m SimpleHTTPServer
~~~

Or, use the [Observable Runtime](https://github.com/observablehq/runtime) to
import this module directly into your application. To npm install:

~~~sh
npm install @observablehq/runtime@4
npm install https://api.observablehq.com/d/a821ebe900c694cc.tgz?v=3
~~~

Then, import your notebook and the runtime as:

~~~js
import {Runtime, Inspector} from "@observablehq/runtime";
import define from "a821ebe900c694cc";
~~~

To log the value of the cell named “foo”:

~~~js
const runtime = new Runtime();
const main = runtime.module(define);
main.value("foo").then(value => console.log(value));
~~~
