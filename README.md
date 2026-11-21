# IoT MUD client template

This is a **starting point, not a working client**. Click **Use this template**
(or fork it) and build your own client in whatever language you like. The
template intentionally contains no client code, so the stack is your choice.

## Start here

1. Read the common server's [BOOTSTRAP.md](https://github.com/FSS-IoT/iot-mud-server/blob/main/BOOTSTRAP.md).
   It walks through creating your repo, running the server, and building the
   smallest client first.
2. Read the protocol: [docs/PROTOCOL.md](https://github.com/FSS-IoT/iot-mud-server/blob/main/docs/PROTOCOL.md).
   This repo targets **version 2** (`PROTOCOL-VERSION`).
3. Run the server locally:

   ```bash
   git clone https://github.com/FSS-IoT/iot-mud-server
   cd iot-mud-server
   uv sync --all-extras
   ./run_server.sh
   ```

4. Build against `SESSION.md`. It is the acceptance test; the copy here is
   pinned, and the [server's copy](https://github.com/FSS-IoT/iot-mud-server/blob/main/docs/SESSION.md)
   is normative.
5. When you are done, replace this README with your client's README: what it
   is, how to run it, and which protocol version it targets.

## The method

The club uses the [software factory](https://fss-iot.github.io/software-factory/)
to build software: brief, spec, tickets, red/green, review, ship. Treat your
client as a small project. The protocol is the spec; `SESSION.md` is the
acceptance test.

- Write a failing check before each step.
- Keep tickets small enough for one session.
- Get a fresh review; the reviewer does not fix your code.
- Ship when `SESSION.md` passes with two players.

## Rules

- Any language, any UI. Terminal, browser, phone, it is your project.
- Offline-first: the game must play with no internet and no LLM.
- Do not copy the server into your client; speak the protocol.
- Do not commit server addresses, passwords, `.env` contents, or database
  files.
- Do not change the protocol privately. Propose changes in the server repo so
  every client can adopt them.

## What to keep

- `SESSION.md` — the acceptance session.
- `PROTOCOL-VERSION` — the protocol major version you target (`2`).
- `.gitignore` — extend it for your stack.

## Credit and license

The protocol and server are club work. See the server's
[NOTICE.md](https://github.com/FSS-IoT/iot-mud-server/blob/main/NOTICE.md).
No license has been chosen for the server yet; this template is a starting
point for club members.
