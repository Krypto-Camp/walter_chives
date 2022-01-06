# walter_chives solidity code
```js
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract Chives {
    uint[5] chives;

    constructor() {
        chives = [1, 1, 1, 1, 1];
    }

    function get() public view returns (uint) {
        uint chives_tt = 0;
        for(uint i=0;i<5;i++) {
            chives_tt += chives[i];
        }
        return chives_tt;
    }

    function cut1() public {
        for(uint i=0;i<3;i++) {
            chives[i] = (chives[i] == 0) ? 1 : 0;
        }
    }

    function cut2() public {
        for(uint i=2;i<5;i++) {
            chives[i] = (chives[i] == 0) ? 1 : 0;
        }
    }

    function cut3() public {
        for(uint i=0;i<5;i++) {
            chives[i] = (chives[i] == 0) ? 1 : 0;
        }
    }
}
```
