
- [PotOfGold.sol](code/contracts/PotOfGold.sol)

    [TODO] A: write Trust Model;

    [o] constructor
    [] convert external onlyOwner
        A: call to complex, external-calling, function as an argument to emitting a LogConvert event
    [] convertMultiple external onlyOwner
    [] _convert
        A: L84: passes 0 as `_minTargetAmount` - discuss about a sandwich  attack
    [] _swap
        A: from this Sushi contract, with some changes: https://github.com/sushiswap/sushiswap/blob/4fdfeb7dafe852e738c56f11a6cae855e2fc0046/contracts/SushiMakerKashi.sol#L138
    [o] _toRNBW
        A: this feels unecessary; using _swap + a comment will save a bit of gas and make things more clear
