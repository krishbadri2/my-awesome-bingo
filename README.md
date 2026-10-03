<div align="center">

# Bingo Mixer

### A little less small talk. A lot more “wait, you too?”

Meet people through a quick game of social bingo. Find someone who matches a square, mark it, and connect your way to five in a row.

[**Play the game**](https://krishbadri2.github.io/my-awesome-bingo/game/) · [**Explore the Copilot lab**](workshop/GUIDE.md) · [**Run it locally**](#run-locally)

<br />

</div>

## Make introductions a game

Bingo Mixer turns the first few minutes of a meetup into an easy excuse to start a conversation. The board is filled with friendly prompts: find someone who plays an instrument, has a hidden talent, or has traveled somewhere new. Mark the square when you find your match, then keep going for five in a row.

1. **Pick a prompt.** Scan the board for a person to meet.
2. **Start a conversation.** Ask around until you find a match.
3. **Mark the square.** Connect five in a row to win.

## More than a game

This project is also a hands-on workshop for building with VS Code and GitHub Copilot. Start with the working app, then explore how context engineering, design-first iteration, custom agents, and test-driven development can shape what you build next.

| Workshop | What you'll explore |
| --- | --- |
| [00 · Overview](workshop/00-overview.md) | The project, learning goals, and checklist |
| [01 · Setup & context](workshop/01-setup.md) | Set up the workspace and give Copilot useful context |
| [02 · Design-first frontend](workshop/02-design.md) | Explore and iterate on a new visual direction |
| [03 · Custom Quiz Master](workshop/03-quiz-master.md) | Create custom bingo themes with an agent |
| [04 · Multi-agent development](workshop/04-multi-agent.md) | Build features with TDD and focused agents |

**[Open the complete workshop guide →](workshop/GUIDE.md)**

## Run locally

You'll need [Node.js 22 or later](https://nodejs.org/).

```bash
git clone https://github.com/krishbadri2/my-awesome-bingo.git
cd my-awesome-bingo
npm install
npm run dev
```

Vite prints the local address when the server is ready. To run the project checks and create a production build:

```bash
npm run lint
npm test
npm run build
```

## Publish your copy

GitHub Actions deploys the workshop docs to the Pages root and the game to `/game/` whenever `main` is pushed. In your repository, open **Settings → Pages** and set the source to **GitHub Actions** to enable publishing.

## Find your way around

- [`src/components/`](src/components/) — game screens and bingo board
- [`src/hooks/useBingoGame.ts`](src/hooks/useBingoGame.ts) — game state
- [`src/utils/bingoLogic.ts`](src/utils/bingoLogic.ts) — bingo rules
- [`src/utils/bingoLogic.test.ts`](src/utils/bingoLogic.test.ts) — rules tests
- [`workshop/`](workshop/) — complete workshop, available to read offline
