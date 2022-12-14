🏆 PRIZE OVERVIEW 

💡 Best new subgraph on The Graph Explorer:
🥇 1st prize: $2200
🥈 2nd prize: $800

📈 Best use of existing subgraph(s) on The Graph Explorer:
🥇 1st prize: $1500
🥈 2nd prize: $500

↓ Full Prize Breakdown Here ↓ 
https://bogota.ethglobal.com/prizes


🚀 WORKSHOP

The Graph 🛠 Building decentralized, serverless applications
Time: 5:30 PM – Oct 07, 2022
Location: Workshop Room 3


🔗 IMPORTANT LINKS
Subgraph Explorer on the Hosted Service: https://thegraph.com/hosted-service/
Subgraph Explorer on The Graph Network: https://thegraph.com/explorer
Developer Documentation: https://thegraph.com/docs/
Follow this guide https://thegraph.com/docs/define-a-subgraph to see how to create a subgraph
Other Dev resources: https://thegraph.academy/developers/developer-resources/
OpenZeppelin Contracts Library Subgraphs: https://github.com/OpenZeppelin/openzeppelin-subgraphs and tutorial https://github.com/pranavdaa/OpenZappelin-Subgraph
Full stack guide: react + ethers.js + solidity + hardhat + subgraphs https://dev.to/dabit3/the-complete-guide-to-full-stack-ethereum-development-3j13
Subgraph Building Demos:

All previous workshops https://codex.thegraph.com/#workshops
3 Minute Subgraph Building Demo https://www.dropbox.com/s/yt9ck6e0uhcu1e5/the-graph-quick-demo.mp4?dl=0
1 Hour Subgraph Building Demo https://www.youtube.com/watch?v=coa0Vw47qNc 

Why graph, why indexed:
* preprocess data (like tabular models)
* otherwise you would have to query lots of contracts, expensive

Subgraph Schema: should be close to 
Entities
Relations between Entities
Mapping: Map data
Transform
Aggregate, similar to typescript

Howto:
Create in web
in terminal:
graph init --studio bayc --index-events
pick net
copy contract address
run... 
now we have the subgraph (indexed data)

Created files:
subgraph.yaml 
    in source you can specify a startbloc
Schema.grraphql
bays.ts
-> then u can deploy
graph codegen

Now go to studio
you can authenticate your computer

graph deploy --stuido bayc
(now it is uploading files to IPFS)

What now?
Data is now there, but to gain information
you need to add to mapping code.
i.e.  add timeStamp
-> create again: graph codegen
-> you still need to add it in bayc.ts to make if effective.
    entity.timeStamp = event.block.timestamp

Go to MyQuery