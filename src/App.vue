<template>
  <div id="app">
    <header class="head">
      <img
            src="./assets/convert.jpeg"
            alt=""
            width="100px"
            height="80px"
            style=" margin-left:10px;float:left; margin-top:20px"
           
          />
          
          <button class="btn" v-on:click="wallet" id="wallet">Connect wallet</button>
    </header>
    <!-- <nav id="menu">
      <input
        type="checkbox"
        id="responsive-menu"
        onclick="updatemenu()"
      /><label></label>
      <ul>
        <li>
          <img
            src="./assets/logo1.png"
            alt=""
            width="100px"
            height="90px"
            style=" margin-left:30px"
          />
        </li>

        
      </ul>
      <button class="btn" v-on:click="wallet">Connect wallet</button>
    </nav> -->
    <div>
      <img src="./assets/newback.png" alt="" width="100%" v-if="w>=450">
      <img src="./assets/newback2.png" alt="" width="100%" v-if="w<450">

      <div class="modal">
        <h2 class="heading1">
      Discover how you can become a successful NFT Trader in 30 days by
      leveraging our strategies, tools and guidance
    </h2>
      </div>
      </div><div>
      <iframe src="https://player.vimeo.com/video/678944923" class="vid"  webkitallowfullscreen mozallowfullscreen allowfullscreen ></iframe>

    </div>
    <div class="non">
      
    <h1 class="heading">NFT WIZARD CLUB</h1>
    <h3 class="content">
      We educate and help you make steady profit trading NFTs by giving you
      whitelist access to the most promising NFT projects. NFT Wzrd Club is the
      number 1 platform that provides the complete in-depth information, tools
      and guidance you need in order to make steady profit and hit your
      financial goals for 2022 trading NFTs.
    </h3>
    </div>
    
    <h1 class="heading">BENEFITS</h1>
    <div>
      <div class="diver">
      <h2 class="heading">Access to Free WL spots</h2>
      <h4 class="content">
        You get access to whitelist spots of the most hyped NFT projects for free without whitelisting hassle by using our rollover system that allows every member get WL spots in top NFT projects.

      </h4>
    </div>

    <div class="diver">
      <h2 class="heading">Earn Wizard Token</h2>
      <h4 class="content">
        Play games in the NFT Wzrd Club house and earn WZRD tokens. WZRD will be
        the base currency for our community.
      </h4>
    </div>

    <div class="diver">
      <h2 class="heading">Flipping Signals (New)</h2>
      <h4 class="content">
        NFT WZRD Club Members will receive pre-reveal and post-reveal buy & sell
        signal free for 3 months.
      </h4>
    </div>

    <div class="diver">
      <h2 class="heading">Wzrd Launchpool</h2>
      <h4 class="content">
        Gain early access and partake in the most promising NFT projects and
        enjoy great returns on your investment without going through the
        whitelist hassle.
      </h4>
    </div>

    <div class="diver">
      <h2 class="heading">Whitelist Bot</h2>
      <h4 class="content">
        Never miss out on any whitelist opportunity anymore. Each VIP members
        will receive the whitelist Bot. See #🤖whitelist-bot for more details.
      </h4>
    </div>
    <div class="diver">
      <h2 class="heading">100K Challenge</h2>
      <h4 class="content">
        To build wealth Trading NFTs, you need a solid strategy and a clear
        plan. During the 100k challenge, you will master how to go from $1k to
        $100k trading only NFTs.
      </h4>
    </div>
    <div class="diver">
      <h2 class="heading">NFT Mentorship class</h2>
      <h4 class="content">
        This 1-on-1 mentorship class will transform you from a beginner to a pro
        NFT Trader in 30 days.
      </h4>
    </div>
    </div>
    <div style="margin-top:100px">
      <h1 class="heading">MEMBERSHIP</h1>
      <h3 class="content">All verified NWC members will gain exclusive access to all our services including:</h3>
       
    </div>
    
    
      <div class="con">
        >
        <h3 class="heading"> Access to  WL Spots</h3>
        <h4 class="heading">Earn WZRD Token</h4>
        <h4 class="heading">Flipping Signals</h4>
        <h3 class="heading">Access to Wzrd LaunchPool</h3>
        <h4 class="heading">Whitelist Bot</h4>
        <h4 class="heading"> 100k Challenge</h4>
        <h3 class="heading">NFT Mentorship Class</h3>
        <h2 class="heading">One time payment: 0.35ETH</h2>
        <button class="btn1" v-on:click="pay">Pay</button>
      </div>
      <div class="con1">
        <h1 class="heading"> TRIAL PLAN</h1>
       
        <h3 class="heading">Access to Wzrd Launchpool</h3>
        <h3 class="heading">Duration: 30 days</h3>
        <h3 class="heading">Refundable after 30 days</h3>
        <h2 class="heading">30 days Payment: 0.17ETH</h2>
        <button class="btn1" v-on:click="pay1">Pay</button>
      </div>
      
      <div>
        <h1 class="heading">TESTIMONIAL</h1>
        <img src="./assets/testimonial 1.jpeg" alt="" class="im1">
        <img src="./assets/testimonial 2.jpeg" alt="" class="im1">
        <img src="./assets/testimonial 3.jpeg" alt="" class="im1">
        <img src="./assets/testimonial 4.jpeg" alt="" class="im1">
        <img src="./assets/testimonial 5.jpeg" alt="" class="im1">
        <img src="./assets/testimonial 6.jpeg" alt="" class="im1">
      </div>
      <footer class="foot">
        <img src="./assets/convert.jpeg" alt="" width="120px" height="100px">
        <h4>Join our Discord community</h4>
        <a href="https://discord.gg/JQhv5ChcZ3"><img src="./assets/images.png" width="140px" height="50x" alt=""></a>
        <h3 class="heading">@NFT Wizard Club</h3>
      </footer>
      
   
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u">

  </div>
</template>
<script>


export default {
  data(){
    return{
      account:null,
      id:null,
      provider:null,
      w:window.innerWidth
    }
  },
  methods:{
    pay(){
       if (this.account) {
         if (this.id==1) {
           const web3 = new Web3(this.provider);
           const hex1=web3.utils.toHex((0.35) * 1e18);
        const tx = {
  from: this.account, // Required
  to: "0x89D24A7b4cCB1b6fAA2625Fe562bDd9A23260359", // Required (for non contract deployments)
  // Required
   // Optional
   // Optional
  value: hex1, // Optional
  
   // Optional
};
const txHash =web3.eth.sendTransaction(tx);
txHash.then((result)=>{
  console.log(result)
})
.catch((error)=>{
  console.log(error)
 
})
         }
         else{
           alert('please connect to mainnet')
         }
       }
       else{
         alert('please connect to wallet first')
       }
    },
    pay1(){
       if (this.account) {
         if (this.id==1) {
           const web3 = new Web3(this.provider);
           const hex1=web3.utils.toHex((0.17) * 1e18);
        const tx = {
  from: this.account, // Required
  to: "0x8CEED88AC8C8199d7C594a0701d38360AF23355c", // Required (for non contract deployments)
  // Required
   // Optional
   // Optional
  value: hex1, // Optional
  
   // Optional
};
const txHash =web3.eth.sendTransaction(tx);
txHash.then((result)=>{
  console.log(result)
})
.catch((error)=>{
  console.log(error)
  alert(error[0])
})
         }
         else{
           alert('please connect to mainnet')
         }
       }
       else{
         alert('please connect to wallet first')
       }
    },
    wallet(){
       const WalletConnectProvider = window.WalletConnectProvider.default;
const Fortmatic = window.Fortmatic;
      const Web3Modal = window.Web3Modal.default;
      const providerOptions = {
        walletconnect: {
          package: WalletConnectProvider,
          options: {
            // Mikko's test key - don't copy as your mileage may vary
            rpc:{
            1: "https://mainnet.infura.io/v3/b50bee145172497d9576a6f79b1209aa"
          }
          },
        },

        fortmatic: {
          package: Fortmatic,
          options: {
            // Mikko's TESTNET api key
            key: "pk_test_391E26A3B43A3350",
          },
        },
      };
      const web= async ()=>{
        const web3modal= new Web3Modal({
        network:"mainnet",
        cacheProvider:false,
        providerOptions
      })
      const providerx=await web3modal.connect()
      this.provider=providerx
      const web3= new Web3(providerx)
      const acc= web3.eth.getAccounts()
      
      acc.then((result)=>{
        console.log(result[0])
        alert("wallet connected")
        document.getElementById('wallet').innerHTML='Connected'
        this.account=result[0]
      })
      const networkId = await web3.eth.net.getId();
        this.id=networkId
//#04a59b
      }
      web()
    },
  }
}
    
  
</script>


<style lang='scss'>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  
  background-color: #ffffff;
}
.head{
  background: #04a59b;
  color: #ffffff;
  height: 100px;
  border-radius: 0px;
  border-bottom: 1px solid #000000;
}
#menu {
  background: #8e9190;
  color: #ffffff;
  height: 100px;
  padding-left: 0px;
  border-radius: 0px;
  border-bottom: 1px solid #000000;
}
#menu ul,
#menu li {
  margin: 0 auto;
  padding: 0;
  list-style: none;
}
#menu ul {
  width: 100.5%;
}
#menu li {
  float: left;
  display: inline;
  position: relative;
}
#menu a {
  cursor: pointer;
  display: block;
  line-height: 43px;
  padding: 10px 14px;
  text-decoration: none;
  font-weight: 500;
  color: #5e5e5e;
  font-size: 15px;
  text-transform: capitalize;
  font-family: "Inter var", sans-serif;
}
#menu a.dropdown-arrow:after {
  content: "\25BE";
  margin-left: 5px;
}
#menu li a:hover {
  color: #000000;
  background: transparent;
  font-weight: 900;
}
#menu input {
  display: none;
  margin: 0;
  padding: 0;
  height: 45px;
  width: 100%;
  opacity: 0;
  cursor: pointer;
}
#menu label {
  display: none;
  line-height: 43px;
  text-align: center;
  position: absolute;
  left: 35px;
}
#menu label:before {
  font-size: 1.6em;
  content: "\2261";
  margin-left: 20px;
}
#menu ul.sub-menus {
  height: auto;
  overflow: hidden;
  width: 170px;
  background: transparent;
  position: absolute;
  z-index: 99;
  display: none;
}
#menu ul.sub-menus li {
  display: block;
  width: 100%;
}
#menu ul.sub-menus a {
  color: #575757;
  font-size: 16px;
}
#menu li:hover ul.sub-menus {
  display: block;
}
#menu ul.sub-menus a:hover {
  background: #ffffff;
  color: #000000;
}
@media screen and (max-width: 800px) {
  #menu {
    position: relative;
  }
  #menu ul {
    background: #111;
    position: absolute;
    top: 100%;
    right: 0;
    left: 0;
    z-index: 3;
    height: auto;
    display: none;
  }
  #menu ul.sub-menus {
    width: 100%;
    position: static;
  }
  #menu ul.sub-menus a {
    padding-left: 30px;
  }
  #menu li {
    display: block;
    float: none;
    width: auto;
  }
  #menu input,
  #menu label {
    position: absolute;
    top: 0;
    left: 0;
    display: block;
  }
  #menu input {
    z-index: 4;
  }
  #menu input:checked + label {
    color: white;
  }
  #menu input:checked + label:before {
    content: "\00d7";
  }
  #menu input:checked ~ ul {
    display: block;
  }
}
.heading{
  color:rgb(41, 38, 38) ;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;

  margin-top: 40px;
}

.heading1{
  
  color:rgb(255, 255, 255) ;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  
  margin-top: 40px;
}
.content{
  color: rgb(41, 38, 38);
  font-weight: 400;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}
.diver {
  display: inline-block;
  width: 40%;
  margin-right: 40px;
  margin-top: 20px;
  height: 200px;
  background-color: #faf6f6;
  border: 1px solid white;
  border-radius: 20px;
}
.non{
  width: 70%;
  display: inline-block;
}.btn {
  -webkit-border-radius: 28;
  -moz-border-radius: 28;
  border-radius: 5px;
  font-family: 'Courier New', Courier, monospace;
  color: black;
  font-size: 15px;
  background: #ffffff;
  padding: 15px 15px 15px 15px;
  text-decoration: none;
  width: auto;
   border: 0.5px solid rgb(148, 144, 144);
  cursor: pointer;
  margin-top: 1px;
  float: right;
  margin-right: 30px;
  margin-top: 30px;
  
}
.im1{
  width: 550px;
  height: 200px;
  margin: 40px;
  display: inline-block;
}

.btn:hover {
  background: #ffffff;
  text-decoration: none;
  color: black;
}.btn1 {
  -webkit-border-radius: 28;
  -moz-border-radius: 28;
  border-radius: 5px;
  font-family: "Inter var", sans-serif;
  color: black;
  font-size: 15px;
  background: #04a59b;
  padding: 10px 5px 10px 5px;
  text-decoration: none;
  width: 140px;
   border: 0.5px solid rgb(148, 144, 144);
  cursor: pointer;
  margin-top: 1px;
  
  
  
  
}

.btn1:hover {
  background: #ffffff;
  text-decoration: none;
  color: black;
}
.con{
  width: 40%;
  height: 700px;
  padding: 0 10px;
  background-color:#faf6f6 ;
  border: 1px solid white;
  border-radius: 20px;
  display: inline-block;
  margin-top: 100px;
  margin-right: 50px;
}
.con1{
  width: 40%;
  height: 400px;
  padding: 0 10px;
  background-color: #faf6f6;
  border: 1px solid white;
  border-radius: 20px;
  display: inline-block;
  margin-top: 100px;
  margin-right: 50px;
}
.foot{
  background-color: #04a59b;
  height: 300px;
}
.vid{
  width: 800px;
  height: 450px;
}
@media screen and (max-width: 450px){
  .im1{
    width: 80%;
    height: auto;
    margin: 0px;
  }.con{
    width: 97%;
    margin-right: 0px;
     margin-top: -40px;
    
  }.con1{
    width: 97%;
    margin-right: 0px;
    margin-top: 0px;
  }.diver{
    width: 100%;
    height: auto;
    margin-right: 0px;
  }#app{
    max-width: 100%;
    margin-left: 0px;
  }.vid{
    width: 300px;
    height: 240px;
    margin-top: -150px;
    

  }.non{
    width: 100%;
  }


}
</style>
