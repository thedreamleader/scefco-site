# Oct 27th 2025, 11:27 PM
when deploying to cloudflare pages, for some reason you need to use bun 1.2.15, while at the time of writing my bun is v1.3.1

bun is not backwards compatible, and therefore build will fail 

solution is either to downgrade to bun 1.2.15 and match cloudflare.. 
or force cloudflare to run 1.3.1 by adding an environment variable during build (BUN_VERSION = 1.3.1)

went with the second one, because first method was having some problems and i am too tired to figure out why
surely this wouldn't come back to bite me or anything haha
in any case, the website's up now, so that's good