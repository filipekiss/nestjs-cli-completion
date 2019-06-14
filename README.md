# [NestJS][nestjs] CLI Completion for ZSH

I've been using [NestJS][nestjs] lately and their [cli][nestjs-cli] is really
handy when it comes to generate new modules, controllers and stuff.

Since I haven't found any shell completion function, I wrote one that suits my
needs.

### Requirements

- zsh

### Installation

1. Clone this repository

```sh
git clone https://github.com/filipekiss/nestjs-cli-completion ~/.completion/nestjs
```

2. Add the path to your `fpath`:

```sh
fpath=(~/.completion/nestjs ${fpath})
```

3. Close your terminal session and start a new one. `nest` command should have
   auto completion now.

### Completion features

- nest commands: **add, generate (g), info (i), new (n) and update (u)**

![image](https://user-images.githubusercontent.com/48519/59521645-269abf80-8ea3-11e9-98ff-82da5bf6fd87.png)

- Argument description, for example, `nest new`

![image](https://user-images.githubusercontent.com/48519/59521670-37e3cc00-8ea3-11e9-9874-e7faf88d8d6f.png)

- Generators auto-complete

![image](https://user-images.githubusercontent.com/48519/59521682-4336f780-8ea3-11e9-9031-39dea6c32f6e.png)

- Short commands (`nest n`, `nest g co`, etc…)

![image](https://user-images.githubusercontent.com/48519/59521697-4c27c900-8ea3-11e9-8088-d40d415a4d63.png)

- Contextual options

![image](https://user-images.githubusercontent.com/48519/59521707-51851380-8ea3-11e9-84b8-a545805eb79f.png)

[nestjs]: https://nestjs.com
[nestjs-cli]: https://github.com/nestjs/nest-cli

## Why no bash completion?

I don't use bash as my main shell and I have no clue how to write bash
completions, sorry. Feel free to write one and make a pull-request, though :)

**nestjs-cli-completion** © 2019+, Filipe Kiss Released under the [MIT] License.<br>
Authored and maintained by Filipe Kiss with help from contributors ([list][contributors]).

> GitHub [@filipekiss](https://github.com/filipekiss) &nbsp;&middot;&nbsp;
> Twitter [@filipekiss](https://twitter.com/filipekiss)

[MIT]: http://mit-license.org/
[contributors]: http://github.com/filipekiss/nestjs-cli-completion/contributors
