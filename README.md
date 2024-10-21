# DanMao Visiter -- Subgraph for DanMao

DanMao is a project developed by FDUBA in 2023. It designed 5000 NFTs by combining "eggshell" elements of FDU with favorable cats in the campus through hand drawing, and the smart contract was deployed on polygon. DanMao achieved a phenomenal success among FDU students once it was published. As a DanMao fan, I wrote this subgraph to track the minting, transfering and collecting of DanMao, in other words, to track DanMao's life. So, are these cyber cats living well?

DanMao contract address(polygon): 0x944cC392Ef48B35631362063F3f2c630CD51AE03

graph init --product subgraph-studio --from-contract 0x944cC392Ef48B35631362063F3f2c630CD51AE03 --network matic --abi "./DanMaoContract/DanMaoAbi.json" DanMaoVisiter

contract name: DanmaoERC721
startBlock: 43564682

> Thanks to Jupiter, who offered a great help when deploying the subgraph. Thanks to Beta for offering the source code of DanMaoContract.

> The DanMao contract is relatively trivial... So the subgraph is as simple as the initial one created by `graph init`.
>
> Maybe I can add something new to DanMaoVisiter later, or I can use The Graph to other scenarios. For example, we can write some smart contract on blockchain to support outsourced computing. In this scenario, there are outsourced computers who should deposit enough money before they accept any outsourced computing task on chain, and the deposit will be transferred to task publisher as compensation if the outsourced computer unintentionally or deliberately submitted wrong result for the task. The Graph can be used in this scenario to track the behavior of all outsourced computers, and rank them based on their average speed of finishing a task, frequency of submitting wrong result and amount of deposit. This will be of significant help to distinguish trustful outsourced computers.
