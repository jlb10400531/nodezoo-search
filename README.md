![Logo](https://raw.githubusercontent.com/nodezoo/nodezoo-org/master/assets/logo-nodezoo.png)

# nodezoo-Search

- __Lead:__ [Richard Rodger][Lead]
- __Sponsor:__ [nearForm][]

Nodezoo Search is an interface with an elasticsearch server. Nodezoo is an example microservice system written in node.js. It is written in a workshop format and designed to help you explore a full microservice
system. Please see the [main repo][] for more details.

## Install
1. Clone this repo into a root _/nodezoo_ folder.
2. Run `npm install`

## Starting
To start simply run,
`npm run start`
       OR
`npm run start-dev`

### Tagging and Logs
To tag your service and set up logs simply pass the relevant switches on start,

```
npm start -- --seneca.options.tag=nodezoo-search --seneca.log.all
```

## Inbound Messages
This micro-service recognizes the following inbound messages:

   * _role:search,cmd:insert_ - insert module details into search engine index
   * _role:search,cmd:search_ - query the search engine

## Outbound Messages
This micro-service emits no outbound messages.

## Contributing
The [NodeZoo org][] encourages __open__ and __safe__ participation.

- __[Code of Conduct]__

If you feel you can help in any way, be it with documentation, examples, extra testing, or new
features please get in touch.
 
## License
Copyright (c) 2014 - 2016, Richard Rodger and other contributors.
Licensed under [MIT][].


[MIT]: ./LICENSE
[Code of Conduct]: https://github.com/nodezoo/nodezoo-org/blob/master/CoC.md
[nearForm]: http://www.nearform.com/
[NodeZoo org]: http://www.nodezoo.com/
[main repo]: https://github.com/rjrodger/nodezoo
[Lead]: https://github.com/rjrodger
