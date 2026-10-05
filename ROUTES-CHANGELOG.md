# Route change log

Which routes are measured has changed, and a share is only comparable over
time if you know when. This file records every addition and removal since the
first run, with the reason.

**A route that was not in the catalog has no zero for that month — it has no
number at all.** Published figures are never back-filled for routes that did
not exist in the run; the run’s own data file lists the routes it measured.

The list below is *computed* from the version history of the route catalog
and of the candidate routes measured alongside it, not maintained by hand:
each recorded state is read and the
difference to the previous one is the event. The reasons are maintained, and
a change without a reason fails the build.

Routes measured today: **37**.

## 2026-08-10 — 33 routes

First catalog, assembled from IANA registries, RFCs, IETF drafts and published vendor conventions.

**Added (33):** `/robots.txt` · `/sitemap.xml` · `/.well-known/security.txt` · `/security.txt` · `/.well-known/api-catalog` · `/.well-known/tdmrep.json` · `/.well-known/gpc.json` · `/.well-known/dnt-policy.txt` · `/.well-known/nodeinfo` · `/.well-known/host-meta` · `/.well-known/ai-catalog.json` · `/.well-known/agent-card.json` · `/.well-known/agent.json` · `/.well-known/mcp.json` · `/openapi.json` · `/.well-known/openapi.json` · `/llms.txt` · `/llms-full.txt` · `/ai.txt` · `/humans.txt` · `/.well-known/ai-plugin.json` · `/ai-plugin.json` · `/agents.txt` · `/agents.json` · `/.well-known/ai-agent.json` · `/ai.json` · `/developer-ai.txt` · `/robots-ai.txt` · `/llm.txt` · `/.well-known/llms.txt` · `/rsl.xml` · `/ads.txt` · `/app-ads.txt`

## 2026-08-10 — 34 routes

One candidate route measured alongside the catalog after the first discovery run found it referenced in the pilot archive; it was dropped again on 12 August with the "comparison yardstick" category.

**Added (1):** `/.well-known/assetlinks.json`

## 2026-08-11 — 29 routes

Evidence review. Seven routes had neither a standing issuer nor a documented consumer and were removed with a written reason; two evidenced routes came in. This revised the earlier position that "a measured zero is a measurement": it holds for formats that have standing, but measuring a route at all lends it a standing it has not earned. For two of the seven the reason names a testable trigger for re-admission (an IANA registration being granted).

**Added (2):** `/.well-known/traffic-advice` · `/.well-known/mcp-server`

**Removed (7):** `/agents.txt` · `/agents.json` · `/.well-known/ai-agent.json` · `/ai.json` · `/developer-ai.txt` · `/robots-ai.txt` · `/llm.txt`

## 2026-08-12 — 33 routes

Four evidenced additions from the registry sweep; /rsl.xml, already measured as a candidate, moved into the catalog.

**Added (4):** `/.well-known/oauth-protected-resource` · `/.well-known/oauth-authorization-server` · `/.well-known/did.json` · `/swagger.json`

## 2026-08-12 — 37 routes

Four evidenced additions from the registry sweep.

**Added (4):** `/.well-known/openid-configuration` · `/.well-known/openid-federation` · `/.well-known/change-password` · `/.well-known/ai.txt`

## 2026-08-12 — 39 routes

Two evidenced additions from the registry sweep.

**Added (2):** `/.well-known/webfinger` · `/.well-known/apple-app-site-association`

## 2026-08-12 — 40 routes

One evidenced addition (payment-capability declaration).

**Added (1):** `/.well-known/x402.json`

## 2026-08-12 — 34 routes

The "comparison yardstick" category was dissolved. Routes that belong to the subject already do that job — /robots.txt (near-complete adoption), /sitemap.xml and /.well-known/security.txt as the RFC-adoption benchmark. Ad verification and app linking added nothing to it but cost one request at every measured host. One further route was dropped on its own ground: it describes the server, not what machines may do with the content.

**Removed (6):** `/.well-known/nodeinfo` · `/.well-known/assetlinks.json` · `/.well-known/change-password` · `/ads.txt` · `/app-ads.txt` · `/.well-known/apple-app-site-association`

## 2026-08-15 — 33 routes

Removed /humans.txt. The file is written for people and says nothing to a machine reader about what may be done with the content — and by convention it names the people involved, which made it the only catalogued route carrying personal data. A route that is not requested cannot raise that question.

**Removed (1):** `/humans.txt`

## 2026-08-25 — 34 routes

The MCP discovery file at the root (/mcp.json) measured alongside the catalog as a candidate — a variant seen in the field next to /.well-known/mcp.json, measured from the September run so the two can be compared.

**Added (1):** `/mcp.json`

## 2026-10-05 — 37 routes

Three candidate routes passed the field threshold (at least three organisations, with a nameable publisher or documented consumer) and are measured from the November 2026 run: the Agent Skills Discovery index (Cloudflare draft), the Universal Commerce Protocol profile, and the MCP server card. Named in the README before the first request.

**Added (3):** `/.well-known/ucp` · `/.well-known/agent-skills/index.json` · `/.well-known/mcp/server-card.json`

---

Routes that were considered and deliberately *not* taken up are recorded with
their reason in the lab; the release lists what is measured and what is under
observation. See [RULESET.md](RULESET.md), section "The route catalog".
