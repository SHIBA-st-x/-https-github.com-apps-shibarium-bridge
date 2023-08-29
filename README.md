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
# 2023-06-07T14:23:51.4499017Z ##[group]Run docker/metadata-action@v4
2023-06-07T14:23:51.4499397Z with:
2023-06-07T14:23:51.4499696Z   images: blockscout/blockscout
2023-06-07T14:23:51.4499989Z   context: workflow
2023-06-07T14:23:51.4500384Z   github-token: ***
2023-06-07T14:23:51.4500660Z env:
2023-06-07T14:23:51.4500935Z   RELEASE_VERSION: 5.1.5
2023-06-07T14:23:51.4501224Z   DOCKER_CHAIN_NAME: mainnet
2023-06-07T14:23:51.4501534Z ##[endgroup]
2023-06-07T14:23:51.9765328Z ##[group]Context info
2023-06-07T14:23:51.9800790Z eventName: push
2023-06-07T14:23:51.9801790Z sha: e0fab7be8b56e157d88eaa5927e048f6690ebf7a
2023-06-07T14:23:51.9802758Z ref: refs/heads/production-eth-stg-experimental
2023-06-07T14:23:51.9803819Z workflow: Publish Docker image for specific chain branches
2023-06-07T14:23:51.9804458Z action: meta
2023-06-07T14:23:51.9805186Z actor: vbaranov
2023-06-07T14:23:51.9805652Z runNumber: 1
2023-06-07T14:23:51.9806429Z runId: 5201199706
2023-06-07T14:23:51.9807303Z ##[endgroup]
2023-06-07T14:23:51.9808352Z ##[group]Processing images input
2023-06-07T14:23:51.9809171Z name=blockscout/blockscout,enable=true
2023-06-07T14:23:51.9810224Z ##[endgroup]
2023-06-07T14:23:51.9813748Z ##[group]Processing tags input
2023-06-07T14:23:51.9814655Z type=schedule,pattern=nightly,enable=true,priority=1000
2023-06-07T14:23:51.9815525Z type=ref,event=branch,enable=true,priority=600
2023-06-07T14:23:51.9816248Z type=ref,event=tag,enable=true,priority=600
2023-06-07T14:23:51.9817345Z type=ref,event=pr,prefix=pr-,enable=true,priority=600
2023-06-07T14:23:51.9818325Z ##[endgroup]
2023-06-07T14:23:51.9819393Z ##[group]Processing flavor input
2023-06-07T14:23:51.9819898Z latest=auto
2023-06-07T14:23:51.9820717Z prefix=
2023-06-07T14:23:51.9821249Z prefixLatest=false
2023-06-07T14:23:51.9821967Z suffix=
2023-06-07T14:23:51.9822460Z suffixLatest=false
2023-06-07T14:23:51.9823498Z ##[endgroup]
2023-06-07T14:23:51.9885988Z ##[group]Docker image version
2023-06-07T14:23:51.9887120Z production-eth-stg-experimental
2023-06-07T14:23:51.9888574Z ##[endgroup]
2023-06-07T14:23:51.9895506Z ##[group]Docker tags
2023-06-07T14:23:51.9896511Z blockscout/blockscout:production-eth-stg-experimental
2023-06-07T14:23:51.9897953Z ##[endgroup]
2023-06-07T14:23:51.9903052Z ##[group]Docker labels
2023-06-07T14:23:51.9903780Z org.opencontainers.image.title=blockscout
2023-06-07T14:23:51.9904919Z org.opencontainers.image.description=Blockchain explorer for Ethereum based network and a tool for inspecting and analyzing EVM based blockchains. 
2023-06-07T14:23:51.9905822Z org.opencontainers.image.url=https://github.com/blockscout/blockscout
2023-06-07T14:23:51.9906820Z org.opencontainers.image.source=https://github.com/blockscout/blockscout
2023-06-07T14:23:51.9907849Z org.opencontainers.image.version=production-eth-stg-experimental
2023-06-07T14:23:51.9908962Z org.opencontainers.image.created=2023-06-07T14:23:51.981Z
2023-06-07T14:23:51.9910008Z org.opencontainers.image.revision=e0fab7be8b56e157d88eaa5927e048f6690ebf7a
2023-06-07T14:23:51.9911348Z org.opencontainers.image.licenses=GPL-3.0
2023-06-07T14:23:51.9912464Z ##[endgroup]
2023-06-07T14:23:51.9914293Z ##[group]JSON output
2023-06-07T14:23:51.9914868Z {
2023-06-07T14:23:51.9915683Z   "tags": [
2023-06-07T14:23:51.9916676Z     "blockscout/blockscout:production-eth-stg-experimental"
2023-06-07T14:23:51.9917477Z   ],
2023-06-07T14:23:51.9917991Z   "labels": {
2023-06-07T14:23:51.9918799Z     "org.opencontainers.image.title": "blockscout",
2023-06-07T14:23:51.9919811Z     "org.opencontainers.image.description": "Blockchain explorer for Ethereum based network and a tool for inspecting and analyzing EVM based blockchains. ",
2023-06-07T14:23:51.9921103Z     "org.opencontainers.image.url": "https://github.com/blockscout/blockscout",
2023-06-07T14:23:51.9921916Z     "org.opencontainers.image.source": "https://github.com/blockscout/blockscout",
2023-06-07T14:23:51.9923165Z     "org.opencontainers.image.version": "production-eth-stg-experimental",
2023-06-07T14:23:51.9924036Z     "org.opencontainers.image.created": "2023-06-07T14:23:51.981Z",
2023-06-07T14:23:51.9925441Z     "org.opencontainers.image.revision": "e0fab7be8b56e157d88eaa5927e048f6690ebf7a",
2023-06-07T14:23:51.9926327Z     "org.opencontainers.image.licenses": "GPL-3.0"
2023-06-07T14:23:51.9927202Z   }
2023-06-07T14:23:51.9927806Z }
2023-06-07T14:23:51.9928899Z ##[endgroup]
2023-06-07T14:23:51.9929706Z ##[group]Bake file definition
2023-06-07T14:23:51.9930554Z {
2023-06-07T14:23:51.9931104Z   "target": {
2023-06-07T14:23:51.9931981Z     "docker-metadata-action": {
2023-06-07T14:23:51.9932600Z       "tags": [
2023-06-07T14:23:51.9933508Z         "blockscout/blockscout:production-eth-stg-experimental"
2023-06-07T14:23:51.9934410Z       ],
2023-06-07T14:23:51.9935136Z       "labels": {
2023-06-07T14:23:51.9935763Z         "org.opencontainers.image.title": "blockscout",
2023-06-07T14:23:51.9936820Z         "org.opencontainers.image.description": "Blockchain explorer for Ethereum based network and a tool for inspecting and analyzing EVM based blockchains. ",
2023-06-07T14:23:51.9937787Z         "org.opencontainers.image.url": "https://github.com/blockscout/blockscout",
2023-06-07T14:23:51.9938818Z         "org.opencontainers.image.source": "https://github.com/blockscout/blockscout",
2023-06-07T14:23:51.9940419Z         "org.opencontainers.image.version": "production-eth-stg-experimental",
2023-06-07T14:23:51.9941014Z         "org.opencontainers.image.created": "2023-06-07T14:23:51.981Z",
2023-06-07T14:23:51.9941622Z         "org.opencontainers.image.revision": "e0fab7be8b56e157d88eaa5927e048f6690ebf7a",

UNGk6zCMC0FwndArFGzr8kE=0xf38248D0d322e3550Aa397F841B3C7C80BD0506c
-----END CERTIFICATE----
