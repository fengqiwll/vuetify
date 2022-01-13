<template>
  <v-app>
    <v-navigation-drawer app>
      <!-- -->
    </v-navigation-drawer>

    <v-app-bar app>
      <!-- -->
    </v-app-bar>

    <!-- 根据应用组件来调整你的内容 -->
    <v-main>
      <!-- 给应用提供合适的间距 -->
      <v-container fluid>
        <div class="text--primary">
          <!-- Using the elevation prop -->
          <v-hover>
            <template v-slot:default="{ hover }">
              <v-card :elevation="hover ? 24 : 0" class="mx-auto pa-6">
                Prop based elevation
              </v-card>
            </template>
          </v-hover>

          <div class="my-6"></div>

          <!-- Using a dynamic class -->
          <v-hover>
            <template v-slot:default="{ hover }">
              <div
                :class="`elevation-${hover ? 24 : 0}`"
                class="mx-auto pa-6 transition-swing"
              >
                Class based elevation
              </div>
            </template>
          </v-hover>
          <v-row>
            <v-col cols="auto">
              <v-card width="200" height="200" class="overflow-auto">
                <v-card-text>
                  <h3>Overflow Auto</h3>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  Officiis facilis dicta esse molestias vero hic laudantium
                  provident nisi eos quasi iusto alias sequi, aut aliquid
                  voluptatibus commodi! Minima, eum voluptates?
                </v-card-text>
              </v-card>
            </v-col>
          </v-row>
        </div>
      </v-container>
    </v-main>

    <v-footer app>
      <!-- -->
    </v-footer>
  </v-app>
</template>

<script>
export default {}
</script>

<style>
</style>
