<template>
  <v-app>
    <v-main>
      <div>
        <v-col>
          <v-card class="mx-auto" max-width="500">
            <v-card-text>
              <div>Please select a db that you want to insert. :)</div>
              <p class="text-h4 text--primary">Chose target Database</p>
            </v-card-text>
            <v-form ref="form" v-model="valid" lazy-validation>
              <v-container fluid>
                <v-radio-group v-model="radios">
                  <template v-slot:label>
                    <div>DB name</div>
                  </template>
                  <v-radio value="MS-SQL-Server">
                    <template v-slot:label>
                      <div>MS SQL Server</div>
                    </template>
                  </v-radio>
                  <v-radio value="Mysql">
                    <template v-slot:label>
                      <div>Mysql</div>
                    </template>
                  </v-radio>
                  <v-radio value="Oracle">
                    <template v-slot:label>
                      <div>Oracle</div>
                    </template>
                  </v-radio>
                  <v-radio value="PostgreSQL">
                    <template v-slot:label>
                      <div>PostgreSQL</div>
                    </template>
                  </v-radio>
                  <v-radio value="MongoDB">
                    <template v-slot:label>
                      <div>MongoDB</div>
                    </template>
                  </v-radio>
                  <v-radio value="Redis">
                    <template v-slot:label>
                      <div>Redis</div>
                    </template>
                  </v-radio>
                  <v-radio value="Elasticsearch">
                    <template v-slot:label>
                      <div>Elasticsearch</div>
                    </template>
                  </v-radio>
                  <v-radio value="Cassandra">
                    <template v-slot:label>
                      <div>Cassandra</div>
                    </template>
                  </v-radio>
                  <v-radio value="MarialDB">
                    <template v-slot:label>
                      <div>MarialDB</div>
                    </template>
                  </v-radio>
                </v-radio-group>
              </v-container>
            </v-form>
          </v-card>
          <v-btn color="warning" @click="content = 'DatabaseChooser'">
            Next step
          </v-btn>
        </v-col>
      </div>
    </v-main>
  </v-app>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "DatabaseChoser",
  data() {
    return {
      radios: "Duckduckgo",
    };
  },
});
</script>
