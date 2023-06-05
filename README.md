# 111-2系統程式 40871228H 廖先翊

## • HW1 https://youtu.be/b2FT_0OTeKc

心智圖連結：https://gitmind.com/app/docs/mptsoro2

<img width="878" alt="截圖 2023-03-07 下午5 55 49" src="https://user-images.githubusercontent.com/104251978/223387615-cde13a52-15c9-4c50-8e51-091924295c5a.png">

- Hardhat :
  - official tutorial : https://hardhat.org/tutorial
  - possible practice (?) : https://medium.com/my-blockchain-development-daily-journey/完整的hardhat實踐教程-a9b005aa4c12

- React JS :
  - official document : https://create-react-app.dev/docs/getting-started/
  - tutorial + practice : https://developer.mozilla.org/zh-TW/docs/Learn/Tools_and_testing/Client-side_JavaScript_frameworks/React_getting_started

- OpenZeppelin :
  - setup official tutorial : https://docs.openzeppelin.com/contracts/4.x/
  - interact with React official tutorial : https://docs.openzeppelin.com/network-js/0.2/building-a-dapp-from-scratch

<br>**Might add some YouTube videos to the above learning lists**

## • HW2 https://youtu.be/wT8J9jZgw6g
影片中最後疑問：
- 不知是否因為版本不同，導致hardhat setup完的整個框架檔案內容(ex. .env.example , .config.js內容)跟數量與老師的示範影片不同，不確定這樣效果會不會不一樣<br>

影片補充 :
- 若.sol裏面import hardhat出現紅字，可以參考[這裡](https://ethereum.stackexchange.com/questions/111568/hardhat-console-cant-be-resolved-in-vscode)
- 最後畫面跑不出來的原因是因為我忘了先執行指令`$ npx hardhat node`，在此補上成果畫面
><img width="500" alt="截圖 2023-04-10 上午12 22 34" src="https://user-images.githubusercontent.com/104251978/230785519-e886f5b7-44cf-4650-ae55-4d45a16a3c35.png">
- 後續：可以從[ERC1155](https://www.openzeppelin.com/contracts)下手研究

## • HW3
- Part1 : https://youtu.be/_UWJfxi32Ks
- Part2 : https://youtu.be/JSqBXT7p8bs
- Figma 專題架構圖：
><img width="600" alt="截圖 2023-05-17 下午5 33 35" src="https://github.com/GavinLiao89/SAD_40871228H/assets/104251978/5d5153fd-c400-431b-97d3-7a361982aa9f"><br>
- 影片中提到的關於metadata，可以使用[Pinata](https://pinata.cloud)

## • HW4 https://youtu.be/ddDaVrMpuLM
><img width="500" alt="截圖 2023-05-17 下午8 48 01" src="https://github.com/GavinLiao89/SAD_40871228H/assets/104251978/7c211a8b-3d8b-46d8-8905-ae2bf2652715">   <img width="500" alt="截圖 2023-05-17 下午9 05 53" src="https://github.com/GavinLiao89/SAD_40871228H/assets/104251978/2f1d036a-fba5-4d69-b548-3a19aeedef14">

- 使用工具 : Alchemy, Pinata, Hardhat, React, Node.js => on Goerli testnet
- 實作目的 : 了解並熟悉前端與後端(ex. solidity合約)的連結方式
- 實作後目標 : 改成上Sepolia testnet測試，並將原先erc721改良成erc1155([implement erc1155Received function](https://forum.moralis.io/t/how-to-implement-erc1155received-function/5492))
- (更新)已成功將Testnet轉換成Sepolia Testnet，以下附上截圖以及說明([官方部分教學](https://docs.alchemy.com/docs/how-to-deploy-a-smart-contract-to-the-sepolia-testnet))：
><img width="500" alt="截圖 2023-05-24 上午12 36 22" src="https://github.com/GavinLiao89/SAD_40871228H/assets/104251978/0de5641f-3b8e-42ce-9d69-c6c04230f021">
><img width="500" alt="截圖 2023-05-24 上午12 36 33" src="https://github.com/GavinLiao89/SAD_40871228H/assets/104251978/3ee7a159-ad04-4cb5-856e-9dfcb15a8d2a">
><img width="500" alt="截圖 2023-05-24 上午12 37 47" src="https://github.com/GavinLiao89/SAD_40871228H/assets/104251978/fe94d8a4-f15c-4610-966d-e517c8c986a7">
><img width="425" alt="截圖 2023-05-24 上午1 30 01" src="https://github.com/GavinLiao89/SAD_40871228H/assets/104251978/75f007da-8f7e-4351-9888-94cf04d05b25">

- (更新)已成功實作將後端ERC-721合約換成ERC-1155版本合約([transfer to non ERC1155Receiver implementer](https://forum.moralis.io/t/how-to-implement-erc1155received-function/5492))


## • Final Presentation https://youtu.be/7q5MOB5BV1c
- 最終Figma流程圖：
><img width="1369" alt="截圖 2023-06-05 下午6 25 42" src="https://github.com/GavinLiao89/SAD_40871228H/assets/104251978/294a7ea6-6457-4639-93d8-5e6eb19a9dae">
- 目前面臨問題(src/NFTMarketplace.sol)：
><img width="1320" alt="截圖 2023-06-05 下午6 25 52" src="https://github.com/GavinLiao89/SAD_40871228H/assets/104251978/e061aa78-939e-4497-8cb0-f2579d0cbeef">
- 補上 ERC-1155 mint NFT 到 Sepolia Testnet的[證明](https://sepolia.etherscan.io/tx/0x06fc132f0574845bc56ccf8e4d34a9159103123a13d7d3f67e97773d0cc4856f)
><img width="1428" alt="截圖 2023-06-05 下午11 21 37" src="https://github.com/GavinLiao89/SAD_40871228H/assets/104251978/312871c9-8f1e-4874-bad2-01272b117564">






# Goal:
- 實作一個線上marketplace，模擬將現今web2的線上課程平台，轉為以web3的方式進行。主要使用hardhat框架，ERC1155智能合約，並在Sepolia Testnet測試。
