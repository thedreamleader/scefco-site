A project/webapp that i build (as a part of my web development learning) for my school's event (unofficially)

Intended to be used for future SCEFCOs as of 2025, comments and documentation will be added to help new developers understand the important parts of the codebase

Problems will be listed here, but if you really want to you can also check "personal_problems.md" but those are more ramblings if anything


- Problem: Cloudflare Pages build fail - "Outdated lockfile version: failed to parse lockfile: 'bun.lockb'"
  - Happens because bun's lockfile is not backwards compatible, you **HAVE** to match versions
  - Cloudflare uses bun 1.2.1 by default
  - Fixed by setting an environment variable "BUN_VERSION = 1.3.1" to force Cloudflare to use 1.3.1
