# Solidity Tutorial
```ad-note
Use remix to compile and write solidity code online.
```

## Syntax of a contract
```solidity
pragma solidity ^0.4.24;

contract MyContract{
	string value;
	function get() public returns(string){
		return value;
	}
	function set(string _value) public {
		value = _value;
	}
}
```



---
# References

<iframe width="560" height="315" src="https://www.youtube.com/embed/ipwxYa-F1uY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
Date: 10-10-2022
Time: 08:49
Status: #note
Tags: #finalyearproject 