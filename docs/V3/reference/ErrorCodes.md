---
id: ErrorCodes
title: Error Codes
---


> LiquidityMath:  Add a signed liquidity delta to liquidity and revert if it overflows or underflows

    > * LS 
    > * LA

Oracle.sol

    * 'OLD': ensure that the target is chronologically at or after the oldest observation

    * 'I': Cardinality must be greater than 0

    * 'I': 'grow' current cardinality must be greater than zero

Position.sol

    * 'NP': disallow pokes for 0 liquidity positions

Tick.sol

    * 'LO' LiquidityGrossAfter must be less than MaxLiquidity

TickMath.sol 

    * 'T':  require(absTick <= uint256(MAX_TICK), 'T');
    * 'R': second inequality must be < because the price can never reach the price at the max tick

TransferHelper.sol

    * 'TF': Transfer failed - errors with TF if transfer fails


UniswapV3Pool.sol

    'LOK'
    TLU
    TLM
    TUM
    X
    AI
    M0
    M1
    AS
    'SPL': Square root price limit
    IIA
    L
    F0
    F1