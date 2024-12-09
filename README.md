# [**View this page on github for it to render properly.**](https://github.com/jsw08/DCBot/blob/master/README.md)

# Jsw's slaafje - my personal Discord bot

![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![Deno JS](https://img.shields.io/badge/deno%20js-000000?style=for-the-badge&logo=deno&logoColor=white)
![Discord](https://img.shields.io/badge/Discord-%235865F2.svg?style=for-the-badge&logo=discord&logoColor=white)

> A relatively simple Discord bot, made with Deno, TS and Discord.JS.

> [!IMPORTANT]
> This bot was made as a learning project that I could use for personal use with
> friends. I have not made it user friendly to install it yourself. It is
> however licensed under the unlicense so you may use the code however you like.

## Commands

| **Command**          | Description                                                                                                                                                                                                                                        | Parameters                                                                                                                                                                                                                                          | Availability                                  | Preview                                                                                                                    |
| -------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| `/ping`              | Responds with "pong"                                                                                                                                                                                                                               | None                                                                                                                                                                                                                                                | Everywhere                                    | ![{6004959A-4792-4FAB-B937-03490B4EF3C0}](https://github.com/user-attachments/assets/c4f5f11b-72dc-4e7f-a77c-9759a0d20ad4) |
| `/time`              | Command to generate Discord Timestamps                                                                                                                                                                                                             | - `time`: REQUIRED string; must be a valid js-datestring.<br>- `type`: REQUIRED autocompleted string; several options for the timestring, including relative, full date etc...                                                                      | Everywhere                                    | ![{82E2C7C6-04AC-43CB-9096-FEDC6951A709}](https://github.com/user-attachments/assets/902b823b-ee6c-4648-9762-80ef40ce4929) |
| `/say`               | Will say something as the bot.                                                                                                                                                                                                                     | You must specify one of these parameters.<br>- `content`: string; the message.<br>- `json`: string; parsed json, use this to add embeds.                                                                                                            | Everywhere                                    | ![{38987594-2F36-483A-BF90-7824D85C7115}](https://github.com/user-attachments/assets/393f6bd6-885d-4a5b-b4c6-fad68319d3d7) |
| Typst                | This set of commands allow you to type and compile typst code in discord. Useful for those moments where you're explaining math to someone.                                                                                                        | Common parameters:<br>- `transparant`: boolean; it'll set the background color of the png to transparant. Only compatible with discord dark mode as the text color will be set to white.<br>- `file`: boolean; it'll attach the typst code as file. | Everywhere                                    | ![image](https://github.com/user-attachments/assets/0b0bc215-b36e-49e4-b76c-7b8c755ca1b8)                                  |
| - `/typst inline`    | You can type one line of typst code within the input itself and it'll generate a picture out of it.                                                                                                                                                | - `code`: REQUIRED string; the typst code.<br>+ common parameters                                                                                                                                                                                   | Everywhere                                    | ![{E0F0DFD8-7853-4E69-91AB-6388FA4B3A5C}](https://github.com/user-attachments/assets/f646dcc7-f2bb-4bfb-9931-2b757e248add) |
| - `/typst multiline` | A modal with a text input will be opened once you run this command so you can type multiple lines of typst code (up to 4000 chars)                                                                                                                 | + common parameters                                                                                                                                                                                                                                 | Everywhere                                    | ![{9AD7B4E8-E139-43B7-890B-1D84F2A3E918}](https://github.com/user-attachments/assets/44331ce4-5d71-44c4-b78f-2aa0edaa4e32) |
| Typescript Eval      | Runs the provided typescript code.                                                                                                                                                                                                                 | Common parameters:<br>- `output`: boolean; if enabled the bot will respond with the input+output of your code in public chat (not ephemeral).                                                                                                       | Nowhere (only configured userids may use it.) | ![{B372D0B4-8DCB-4837-81A6-19178854872F}](https://github.com/user-attachments/assets/c0160e25-662f-48c4-a69b-a9ce5e78bef9) |
| - `/ts inline`       | Allow's for one line of typescript code. So you can either just run simple or minified code.                                                                                                                                                       | - `code`: REQUIRED string; ts code.<br>+ common parameters                                                                                                                                                                                          | Nowhere                                       | ![{7B5BFDEB-31DE-448C-B9BF-AAFF07107176}](https://github.com/user-attachments/assets/51caf1f5-d25b-4dd0-ae60-2a56ddb809b6) |
| - `/ts multiline`    | Opens a modal for longer codesnippets (again max length of 4000 characters).                                                                                                                                                                       | + common parameters                                                                                                                                                                                                                                 | Nowhere                                       | ![{0383FEBD-BEDC-4AFC-A041-7AD657F83914}](https://github.com/user-attachments/assets/426b5148-d8ff-4d4a-b55a-684fca5428a1) |
| Sexy                 | This collection of commands allows me and my friends to - Upload unappealing pictures of eachother to my server. - Send them (within my discord server) using my bot. This allows us to have a central place to store funny pictures of eachother. | Common parameters:<br>- `nickname`: REQUIRED autocompleted string; the nickname under which the photos are stored<br>- `public`: bool; makes the message not ephemeral.                                                                             | At specified guilds                           | ![{3BE5E9E8-78DB-46C2-82A2-E6566A9346A3}](https://github.com/user-attachments/assets/ae42a66a-0103-46dd-a4a4-833132da6dcf) |
| - `/sexy carousel`   | Displays the pictures in a 4x4 grid with scrolling buttons on the bottom                                                                                                                                                                           | - `page`: autocompleted number; specifies the page the carousel should start at.<br>+ common parameters                                                                                                                                             | At specified guilds                           | ![{AFEF4549-058D-4A2A-9728-069BC10B9E88}](https://github.com/user-attachments/assets/973d8fa5-5684-42cb-a423-1701db5ffdea) |
| - `/sexy image`      | Allows you to pick one image to send.                                                                                                                                                                                                              | - `image`: REQUIRED autocompleted string; specifies the iamge that should be displayed.<br>+ common parameters                                                                                                                                      | At specified guilds                           | ![{FC525F05-26AF-428C-AB30-12AB293C6206}](https://github.com/user-attachments/assets/ca525b3e-e862-4f2d-ad2e-d3daf4f125b3) |
| - `/sexy-upload`     | Uploads the specified image to the server's filesystem.                                                                                                                                                                                            | - `nickname`: REQUIRED autocompleted string; the nickname under which the photos are stored<br>- `filename`: REQUIRED string; a name that should describe the image.<br>- `image`: REQUIRED asset; the image file.                                  | At specified guilds                           | ![{ABC3995A-DB63-4DB6-BB42-10251DA4FD53}](https://github.com/user-attachments/assets/d338b22b-b953-47f2-9659-baf9283b153a) |
| LastFM               | These commands show what song you or a lastfm user is currently playing                                                                                                                                                                            | None                                                                                                                                                                                                                                                | Everywhere                                    | ![{C47A3CDE-C134-4209-A861-10E71161B4F9}](https://github.com/user-attachments/assets/081d33cb-09f0-4fd8-ba79-57241aca68c6) |
| `/fm np`             | Gets the currently playing song of either your lastfm username or the provided one.                                                                                                                                                                | - `username`: string; overwrites the lastfm username.                                                                                                                                                                                               | Everywhere                                    | ![{5432B1AF-6237-499C-8DE7-3C5778C2B30F}](https://github.com/user-attachments/assets/4e2d1367-9788-4397-80a0-ae1fd4201873) |
| `/fm set`            | Sets your lastfm user. It alsoc ckecks if the provided username exists.                                                                                                                                                                            | - `username`: REQUIRED string; the username that will be set in the database.                                                                                                                                                                       | Everywhere                                    | ![{93A91DDB-A095-4F93-9B5A-A40F5768E025}](https://github.com/user-attachments/assets/07222deb-e0e4-4784-8414-1a86b8119f3e) |

## Installation

### Prerequisites

- Required
  - Deno
  - Git
  - Port forwarding / a different solution to get the web server online.
- Optional
  - Typst

### Installation

- `git clone https://github.com/jsw08/dcbot`
- `cd dcbot`
- `deno i`

## Configuration

This program works using dotenv. So you can either place a .env file in the
project root, or set the environment variables. See the
[template file](https://github.com/jsw08/DCBot/blob/master/template.env).

## Usage

- Make sure you have your [environment variables](#configuration) set.
- Run `deno run -A ./src/main.ts`

## Screenshots and recordings

![{35FE9E78-CABA-41B1-B861-940C94C80203}](https://github.com/user-attachments/assets/98174ebf-59e3-4f8b-8068-09b4d6c8c7e4)

### Sexy mfs

https://github.com/user-attachments/assets/5ade453d-41c9-430f-893f-04c1c20819b8

### Utilities

https://github.com/user-attachments/assets/1413376d-a00a-4909-a01e-5e86f9cbe201
