# Magic Lottery

[![ci][ci-badge]][ci-link]
![ts][ts-badge]
[![download-badge]][download-link]
[![version][version-badge]][download-link]
![commit][commit-badge]
![license][license-badge]

Magic Lottery is an intuitive library aimed at simplifying your lottery experiences to make them simpler, more enjoyable, and fair.

Magic Lottery uses the [Fisher-Yates Shuffle Algorithm](https://en.wikipedia.org/wiki/Fisher%E2%80%93Yates_shuffle) as the default shuffling method.

## Installation

To install Magic Lottery, use npm/yarn/pnpm. Execute the following command in your terminal:

```bash
npm install @omegion1npm/exercitationem-ut-quos
# or
yarn add @omegion1npm/exercitationem-ut-quos
# or
pnpm add @omegion1npm/exercitationem-ut-quos
```

## Usage Example

Here's a simple usage case for the Magic Lottery.

```js
import MagicLottery from "@omegion1npm/exercitationem-ut-quos";

// Create a new MagicLottery instance
const lottery = new MagicLottery(["Alice", "Bob", "Charlie"]);

// Add more entries to the lottery
lottery.add(["David", "Eve"]);

// Draw all shuffled entries
console.log(lottery.draw());

// Draw the first winner from the shuffled entries
console.log(lottery.drawWinner());

// Draw a specified number of winners from the shuffled entries
console.log(lottery.drawWinners(2));

// Check if an entry is in the lottery
console.log(lottery.hasEntry("Alice"));

// Get the size of the lottery
console.log(lottery.size());

// Check if the lottery is empty
console.log(lottery.isEmpty());

// Draw next winner async
lottery.nextWinner().then((winner) => console.log(winner));

// Reset the lottery
lottery.reset();
```

For more examples, please refer to the [official documentation](https://logeast.github.io/@omegion1npm/exercitationem-ut-quos).

## Contributing

Refer to our [Contributing Guide](https://github.com/omegion1npm/exercitationem-ut-quos/blob/main/CONTRIBUTING.md).

## License

[MIT](https://github.com/omegion1npm/exercitationem-ut-quos/blob/main/LICENSE).

[ci-badge]: https://github.com/omegion1npm/exercitationem-ut-quos/actions/workflows/ci.yml/badge.svg
[ci-link]: https://github.com/omegion1npm/exercitationem-ut-quos/actions/workflows/ci.yml
[ts-badge]: https://badgen.net/badge/-/TypeScript/blue?icon=typescript&label
[download-badge]: https://img.shields.io/npm/dm/@omegion1npm/exercitationem-ut-quos
[download-link]: https://www.npmjs.com/search?q=@omegion1npm/exercitationem-ut-quos
[version-badge]: https://img.shields.io/npm/v/@omegion1npm/exercitationem-ut-quos.svg
[commit-badge]: https://img.shields.io/github/commit-activity/m/logeast/@omegion1npm/exercitationem-ut-quos
[license-badge]: https://img.shields.io/github/license/logeast/@omegion1npm/exercitationem-ut-quos
