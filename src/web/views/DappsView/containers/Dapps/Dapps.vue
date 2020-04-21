<template>
  <WhiteSheet>
    <Banner />
    <div class="px-8 py-5">
      <DappsButton v-for="dapp in dapps" :key="dapp.id" :data="dapp" />
    </div>
  </WhiteSheet>
</template>

<script>
import WhiteSheet from '@/web/components/Common/WhiteSheet';
import Banner from './components/Banner';
import DappsButton from '@/components/DappsButton';

import IconMakerDAO from '@/assets/images/icons/dapps/icon-maker-dai.svg';
import IconEnsManager from '@/assets/images/icons/dapps/icon-ens-manager.svg';
import IconSafeSendTx from '@/assets/images/icons/dapps/icon-safe-send-tx.svg';

export default {
  components: { WhiteSheet, Banner, DappsButton },
  data() {
    return {
      dapps: [
        {
          name: 'MakerDAO',
          description: 'Collateralize & Generate DAI',
          hashTags: ['Exchanges'],
          img: IconMakerDAO
        },
        {
          name: 'ENS manager',
          description: 'Migrate or register ENS domain / subdomain',
          hashTags: ['Property'],
          img: IconEnsManager
        },
        {
          name: 'SafeSend Transaction',
          description: 'Protect & secure your ETH transaction',
          hashTags: ['Security'],
          img: IconSafeSendTx
        }
      ]
    };
  }
};
</script>
