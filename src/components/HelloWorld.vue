<template>
  <div>
    <v-container class="plan-list">
      <v-layout text-center>
        <v-flex xs3>
          <v-card>
            <v-card-title class="plan-title-bg">
              <v-layout text-center>
                <v-flex class="plan-title">
                  <p>Free</p>
                  <p class="title-description">テスト向け</p>
                </v-flex>
              </v-layout>
            </v-card-title>
            <v-card-text class="plan-price">
              <v-layout text-center>
                <v-flex md6 class="plan-title">
                  <section>
                  <p>月額課金</p>
                  </section>
                  <section>
                  </section>
                </v-flex>
                <v-flex md6 class="plan-title" style="border-left: 3px solid;">
                  <section>
                  <p>従量課金</p>
                  </section>
                  <section>
                  </section>
                </v-flex>
              </v-layout>
            </v-card-text>
            <v-card-actions>
              <v-layout text-center>
                <v-flex md6 offset-md-3>
                  <v-btn color="success" depressed small>Normal</v-btn>
                </v-flex>
              </v-layout>
            </v-card-actions>
          </v-card>
        </v-flex>
        <v-flex xs3>
          <v-card>
            <v-card-title class="plan-title-bg">
              <v-layout text-center>
                <v-flex class="plan-title">
                  <p>Free</p>
                  <p class="title-description">サイト埋め込み向け</p>
                </v-flex>
              </v-layout>
            </v-card-title>
            <v-card-text class="plan-price">
              <v-layout text-center>
                <v-flex md6 class="plan-title">
                  <section>
                    <p>月額課金</p>
                  </section>
                  <section>
                  </section>
                </v-flex>
                <v-flex md6 class="plan-title" style="border-left: 3px solid;">
                  <section>
                  <p>従量課金</p>
                  </section>
                  <section>
                  </section>
                </v-flex>
              </v-layout>
            </v-card-text>
            <v-card-actions>
              <v-layout text-center>
                <v-flex md6 offset-md-3>
                  <v-btn color="success" depressed small>Normal</v-btn>
                </v-flex>
              </v-layout>
            </v-card-actions>

          </v-card>
        </v-flex>
        <v-flex xs3>
          <v-card>
            <v-card-title class="plan-title-bg">
              <v-layout text-center>
                <v-flex class="plan-title">
                  <p>Prime</p>
                  <p class="title-description">広告配信向け</p>
                </v-flex>
              </v-layout>
            </v-card-title>
            <v-card-text class="plan-price">
              <v-layout text-center>
                <v-flex md6 class="plan-title">
                  <section>
                  <p>月額課金</p>
                  </section>
                  <section>
                  </section>
                </v-flex>
                <v-flex md6 class="plan-title" style="border-left: 3px solid;">
                  <section>
                  <p>従量課金</p>
                  </section>
                  <section>
                  </section>
                </v-flex>
              </v-layout>
            </v-card-text>
            <v-card-actions>
              <v-layout text-center>
                <v-flex md6 offset-md-3>
                  <v-btn color="success" depressed small>Normal</v-btn>
                </v-flex>
              </v-layout>
            </v-card-actions>

          </v-card>
        </v-flex>
        <v-flex xs3>
          <v-card>
            <v-card-title class="plan-title-bg">
              <v-layout text-center>
                <v-flex class="plan-title">
                  <p>Pro</p>
                  <p class="title-description">大規模広告配信向け</p>
                </v-flex>
              </v-layout>
            </v-card-title>
            <v-card-text class="plan-price">
              <v-layout text-center>
                <v-flex md6 class="plan-title">
                  <section>
                  <p>月額課金</p>
                  </section>
                  <section>
                  </section>
                </v-flex>
                <v-flex md6 class="plan-title" style="border-left: 3px solid;">
                  <section>
                  <p>従量課金</p>
                  </section>
                  <section>
                  </section>
                </v-flex>
              </v-layout>

              <v-layout text-center>
                <v-flex>
                  <p style="font-weight: 700;">お問い合わせください</p>
                  <p style="font-size: 70%;">※クリックすると、<br>フォームを別タブで表示します。</p>
                </v-flex>
              </v-layout>
            </v-card-text>
            <v-card-actions>
              <v-layout text-center>
                <v-flex md6 offset-md-3>
                  <v-btn color="error" depressed small>お問い合わせ</v-btn>
                </v-flex>
              </v-layout>
            </v-card-actions>

          </v-card>
        </v-flex>
      </v-layout>
    </v-container>
    <v-dialog v-model="dialog" width="900" >
      <template v-slot:activator="{on}">
        <span v-on="on">Open Dialog</span>
      </template>
      <v-card>
        <v-simple-table fixed-header>
          <thead>
            <tr>
              <th colspan="2" class="text-center">Name</th>
            </tr>
          </thead>
          <tbody>
            <tr v-for="item in desserts" :key="item.name" class="text-center">
              <td width="50%">{{ item.name }}</td>
              <td width="50%">{{ item.calories }}</td>
            </tr>
          </tbody>
        </v-simple-table>
      </v-card>
    </v-dialog>
  </div>
</template>

<style lang="scss" scoped>
  tr:nth-child(odd):hover {
    background-color: #E1E1E1 !important;
  }
  tr:nth-child(odd) {
    background-color: #E1E1E1;
  }
  tr:nth-child(even):hover {
    background-color: #5d5d5d !important;
  }
  tr:nth-child(even) {
    background-color: #5d5d5d;
  }
  .plan-list p {
    margin: 0;
    color: rgba(0,0,0,.87) !important;
  }
  .plan-title {
    font-weight: 700;
  }
  .title-description {
    font-size: 70%;
  }
  .plan-title-bg {
    background-color: #E1E1E1;
  }
  .plan-price {
    padding: 0;
  }
</style>

<script>
export default {
  data() {
    return {
        desserts: [
          {
            name: 'Frozen Yogurt',
            calories: 159,
          },
          {
            name: 'Ice cream sandwich',
            calories: 237,
          },
          {
            name: 'Eclair',
            calories: 262,
          },
          {
            name: 'Cupcake',
            calories: 305,
          },
          {
            name: 'Gingerbread',
            calories: 356,
          },
          {
            name: 'Jelly bean',
            calories: 375,
          },
          {
            name: 'Lollipop',
            calories: 392,
          },
          {
            name: 'Honeycomb',
            calories: 408,
          },
          {
            name: 'Donut',
            calories: 452,
          },
          {
            name: 'KitKat',
            calories: 518,
          },
        ],
    dialog: false,
    ecosystem: [
      {
        text: 'vuetify-loader',
        href: 'https://github.com/vuetifyjs/vuetify-loader',
      },
      {
        text: 'github',
        href: 'https://github.com/vuetifyjs/vuetify',
      },
      {
        text: 'awesome-vuetify',
        href: 'https://github.com/vuetifyjs/awesome-vuetify',
      },
    ],
    importantLinks: [
      {
        text: 'Documentation',
        href: 'https://vuetifyjs.com',
      },
      {
        text: 'Chat',
        href: 'https://community.vuetifyjs.com',
      },
      {
        text: 'Made with Vuetify',
        href: 'https://madewithvuejs.com/vuetify',
      },
      {
        text: 'Twitter',
        href: 'https://twitter.com/vuetifyjs',
      },
      {
        text: 'Articles',
        href: 'https://medium.com/vuetify',
      },
    ],
    whatsNext: [
      {
        text: 'Explore components',
        href: 'https://vuetifyjs.com/components/api-explorer',
      },
      {
        text: 'Select a layout',
        href: 'https://vuetifyjs.com/layout/pre-defined',
      },
      {
        text: 'Frequently Asked Questions',
        href: 'https://vuetifyjs.com/getting-started/frequently-asked-questions',
      },
    ],
  }},
};
</script>
