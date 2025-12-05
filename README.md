# base33h
Deploying Smart Contracts on Base With Hardhat &amp; Verifying Automatically
A best practice is to verify contracts automatically via scripts.
Base supports Etherscan-compatible verification.

JS example verification script

async function verify(address) {
  await hre.run("verify:verify", {
    address,
    constructorArguments: []
  });
}
