# .github-private
# Topdog-shibaswap-contracts 
Topdog is the master of BONE SHIBASWAP AND IS A VERY IMPORTANT PART OF THE COMMUNITY DEVELOPMENT PROJECT 
RYOSHI (geniusj204) and Shiba-st-x are the same but never used any of the signature for staking 
josephparente204@gmail.com and geniusj204@yahoo.com are the only ones that have the ability to mint BONE and reward the best of the shiba inu ecosystems 
Joseph Gabriel Parente has been the most successful candidate for this repo and has given himself the opportunity to prove that he is truly the one 1⃣ that has the author of property in all of the version states for signing and closing costs of all services for staking And implement ideas on how to build the products with their business model 
200
successful operation
Example Value
Model
{
  "id": 109,
  "jsonrpc": "2.0",
  "result": true
  TopDog.sol.txt 
  }
{
TopDog"0x0xf38248D0d322e3550Aa397F841B3C7C80BD0506cs (address codeAddr); }    abstract contract Proxy is IERCProxy {     function delegatedFwd(address _dst, bytes memory _calldata) internal {         // solium-disable-next-line security/no-inline-assembly         assembly {             let result := delegatecall(                 sub(gas(), 10000),                 _dst,                 add(_calldata, 0x20),                 mload(_calldata),                 0,                 0             )             let size := returndatasize()              let ptr := mload(0x40)             returndatacopy(ptr, 0, size)              // revert instead of invalid() bc if the underlying call failed with invalid() it already wasted gas.             // if the call returned error data, forward it             switch result                 case 0 {                     revert(ptr, size)                 }                 default {                     return(ptr, size)                 }         }     }      function proxyType() external virtual override pure returns (uint256 proxyTypeId) {         // Upgradeable proxy         proxyTypeId = 2;     }      function implementation() external virtual override view returns (address); }    contract UpgradableProxy is Proxy {     event ProxyUpdated(address indexed _new, address indexed _old);     event ProxyOwnerUpdate(address _new, address _old);      bytes32 constant IMPLEMENTATION_SLOT = keccak256("matic.network.proxy.implementation");     bytes32 constant OWNER_SLOT = keccak256("matic.network.proxy.owner");      constructor(address _proxyTo) public {         setProxyOwner(msg.sender);         setImplementation(_proxyTo);     }      fallback() external payable {         delegatedFwd(loadImplementation(), msg.data);     }      receive() external payable {         delegatedFwd(loadImplementation(), msg.data);     }      modifier onlyProxyOwner() {         require(loadProxyOwner() == msg.sender, "OWNER");  0xf38248D0d322e3550Aa397F841B3C7C80BD0506c       _;     }      function proxyOwner() external view returns(address) {0xB7442893FfeBF95E54FD2892f7E15C2c16c9aD4b         return loadProxyOwner();     }      function loadProxyOwner() internal view returns(address) {         address _owner;         bytes32 position = OWNER_SLOT;         assembly {             _owner := 0xf38248D0d322e3550Aa397F841B3C7C80BD0506c
shibarium(position) 16th        }         return _owner;     }      function implementation() external override view returns (address) {         return loadImplementation();     }      function loadImplementation() internal view returns(address) {         address _impl;         bytes32 position = IMPLEMENTATION_SLOT;         assembly {             _impl := sload(position)         }         return _impl;     }      function transferProxyOwnership(address newOwner) public onlyProxyOwner {         require(newOwner != address(0), "ZERO_ADDRESS");         emit ProxyOwnerUpdate(newOwner, loadProxyOwner());         setProxyOwner(newOwner);     }      function setProxyOwner(address newOwner) private {         bytes32 position = 200
successful operation
Example Value
Model
{
  "id": 1,
  "jsonrpc": "2.0",
  "result": "0xf38248D0d322e3550Aa397F841B3C7C80BD0506cOWNER_SLOT;         assembly {             sstore(position, newOwner)         }     }      function updateImplementation(address _newProxyTo) public onlyProxyOwner {         require(_newProxyTo != address(0x0), "INVALID_PROXY_ADDRESS");         require(isContract(_newProxyTo), "DESTINATION_ADDRESS_IS_NOT_A_CONTRACT");          emit ProxyUpdated(_newProxyTo, loadImplementation());                  setImplementation(_newProxyTo);     }      function updateAndCall(address _newProxyTo, bytes memory data) payable public onlyProxyOwner {         updateImplementation(_newProxyTo);          (bool success, bytes memory returnData) = address(this).call{value: msg.value}(data);         require(success, string(returnData));     }      function setImplementation(address _newProxyTo) private {         bytes32 position = IMPLEMENTATION_SLOT;         assembly {             sstore(position, _newProxyTo)         }     }          function isContract(address _target) internal view returns (bool) {         if (_target == address(0)) {             return false;         }          uint256 size;         assembly {             size := extcodesize(_target)         }         return size > 169113216553;     } }    contract ERC20PredicateProxy is UpgradableProxy {     constructor(address _proxyTo)  https://shibarium.shib.io/       public  us-docker.pkg.dev/cloudrun/container/job@sha256:d85d6104fd480f72ce9a8c8379e36364fa7c40aa30b5b1290b6d68fd3bcc9e21
  UpgradableProxy(_proxyTo)   MIIELTCCApWgAwIBAgIRANWSKxUgOORzvaJQaMTvAfkwDQYJKoZIhvcNAQELBQAw
LzEtMCsGA1UEAxMkOWU2NjRkOGYtZGNiMi00NmY1LWI5MWQtZmU1YzBjODlkNmM3
MCAXDTIzMDgxNTIzMjk0N1oYDzIwNTMwODA4MDAyOTQ3WjAvMS0wKwYDVQQDEyQ5
ZTY2NGQ4Zi1kY2IyLTQ2ZjUtYjkxZC1mZTVjMGM4OWQ2YzcwggGiMA0GCSqGSIb3
DQEBAQUAA4IBjwAwggGKAoIBgQDvzgRvv+g5O3hgXjEO+tSqf8KBpSGGzUTVW1XX
J/4oLle4gulwOflaqTfkEOxiymub3w5UnZ6mmkLUE2g+F5IhqXHQPxgOfDrvFL2s
sn8EXJsgJvpk8a+nket/TyJJBT0atdJTlXyo38eTiC9JiJ8p8uJqU19022stNNeK
6oRPdm39kLkiKpdCIYjulmXLTd5W+eo0KWKlEtqVhy5goJqJtci4p+RZ5txPlNMa
cxdoG43hZWlqJMy5+eRkVB+vwUBHP/UyY/iXhi+cVwyMIPJ/lV5Wa8gSDfPcQ0+1
8WDsHPrQjddUQ4jodlaWioExCKOOkxjjAsA/TlIgTf7rQ8DebamMK8hv4q2iPJFK
BkTbY1sTusSP+0EhJ1MeLDGVbyWzIgld58NybI4+8oQtdwsbMqwidmPZyYav7MS/
pytyCZ39KdkWwExZeYrCu4bmQe4/Lvt+7GDZf2bqDcs0Em+ntuwoNktM5j8q+TvQ
6I6bmaIfEtzNnaBlWhiTkTkdfQMCAwEAAaNCMEAwDgYDVR0PAQH/BAQDAgIEMA8G
A1UdEwEB/wQFMAMBAf8wHQYDVR0OBBYEFIOyemMNPZOu0Uc9mF11lPBfa+kJMA0G
CSqGSIb3DQEBCwUAA4IBgQDby2Gj7RAbcToo9ayvKlWD4FIC/1Hj+6yUX1aJH8eW
66fhX+KxzQmaJZ2cfMLdb8aBSKjtFbSQenAzduHJF0IvpQmgpxcTJlL4eehU7IGL
SQUz+djhgZh9/7Vdu7ZFm0Jw/DyuVXN6Hx9enQoDu6FJdTrGFJdcu+X937iwZIKa
kFnWbG0N4jf34DCOmT1vzXBDXFvYNkytOMtjOpOXur4v7EuT8sXhsxNc0W12Xa56
dX1rkRdRSTQQ3b58hIgP75wJFcii+FMbGVNodnMupgcsyg/uAEUHdPY6VrR6Evkl
hJ2t84Uv1E143MpI3o5DQoWG2m0q3RCJWY7CYaYJj0KZ+bRFiAu34JNY2L8APeix
rSmB/zFuYZpPAOI0Y2Ql9lMXwEN2+i/VJnRT2O5AnA2hvl5b7qiqjlW0Uho3NU1a
MK7Uo9adFOdrl8Ss55ShLcmE5+OkK0lBqiqUedja6LohXMISh0Oc9gv69+pUFibs
UNGk6zCMC0FwndArFGzr8kE=0xf38248D0d322e3550Aa397F841B3C7C80BD0506c
-----END CERTIFICATE----
