# Prunecress 1.0 TEST
Native Android weighted directed feedback vertex set puzzle. Android8+ min26/target35. Package com.gg007.prunecress.

## Rules
Seven nodes A-G have positive removal costs and directed outgoing-arrow lists. If row A lists CF, the arrows are A to C and A to F, not the reverse. Tap a node row to toggle KEEP and REMOVED. Removing a node deletes that node and every arrow entering or leaving it. Among the kept nodes, no directed cycle may remain. A directed cycle follows arrows and returns to its starting node. The remaining graph need not be connected or a tree. Minimize the sum of removed-node costs, not the number of removed nodes. CHECK NETWORK explicitly; any minimum-cost removal set is accepted. Twelve original graphs, each with no reciprocal arrow pairs and one minimum-cost set. Undo, reset and saved palette/node-number settings. This is a weighted directed feedback vertex set puzzle.

## Download
https://mega.co.nz/#!lRsjmLTa!FvFlXIcwDWCl0-irD-BJRQw8rBjZD_28nlDQ4jWdato
{"url": "https://mega.co.nz/#!lRsjmLTa!FvFlXIcwDWCl0-irD-BJRQw8rBjZD_28nlDQ4jWdato", "bytes": 16878, "sha256": "eea17a77cd2421baaf190304382f040fbe79dd176b7ca38877c76ca6501545d9", "anonymous_bytes_exact": true}

## Checks
An independent Floyd-style transitive-closure oracle agrees with production Kahn source-elimination cycle tests on all 1,536 shipped subsets, plus every subset of 2,000 random graphs. All 10,752 node-toggle/undo cases pass. The optimum cost and exact CHECK acceptance agree for every shipped subset. Empty, single, self-loop, directed path, triangle, disconnected cycles, zero-cost and out-of-bounds cases pass. Twelve actual node-toggle/CHECK minimum-cost tap-solves, cyclic-start rejection, undo/reset, solved lock/NEXT, levels/menu/privacy and saved palette/node numbers pass. Twenty drawing previews inspected, not phone screenshots. Original signing certificate and GG007 icon bytes unchanged; no permissions. Anonymous APK bytes match. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
The live 245 studio descriptions and 803 legacy descriptions were reviewed. Guardcress selects pairwise nonconflicting vertices to maximize reward; Graftcress selects undirected spanning-tree edges; Arrowhaven chooses directions to reach a goal. Prunecress removes weighted directed vertices to destroy every directed cycle while keeping the cheapest total removal. Every shipped graph has no reciprocal arrow pairs: every two-node subgraph is already acyclic, but larger cycles remain. It is not a pair-conflict selection reskin. Known directed feedback vertex set adaptation, not a globally new algorithm. Twelve original seeded graphs, native implementation and kept/removed-node interaction.

## Build and tests
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/prune-test src/com/gg007/prunecress/Board.java BoardTest.java then java -cp /tmp/prune-test com.gg007.prunecress.BoardTest. bash build.sh produces an aligned unsigned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to private signing material. No signing secret included. adapter/android is a Java2D drawing adapter used with PruneAdapterTest.java, not an Android runtime.

## Privacy and branding
Prunecress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, node-number labels and solved-level marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 icon/menu/studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK/exact cumulative246-card studio/publishing fragments privately preserved:
https://files.instinct.com/omkmx6k11tm0-prunecress-source-archive
https://github.com/iLanis-agent/prunecress holds README only; full Git source pending. Four studio includes and Pages settings unchanged. Both sites verified separately.

## Rule sources
https://arxiv.org/html/2311.01026v3
https://pacechallenge.org/2022/directed-fvs/
http://www.diag.uniroma1.it/~demetres/docs/mfas.pdf
https://drops.dagstuhl.de/storage/00lipics/lipics-vol249-ipec2022/LIPIcs.IPEC.2022.28/LIPIcs.IPEC.2022.28.pdf
https://arxiv.org/abs/2208.01119
https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.dag.is_directed_acyclic_graph.html
