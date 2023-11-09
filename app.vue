<template>
  <!-- <div class="login-root">
    <div
      class="box-root flex flex-direction--column"
      style="min-height: 100vh; flex-grow: 1"
      const existingDataIndex = this.kapalData.findIndex((item) => {
    >
      <div class="loginbackground box-background--white padding-top--64">
        <div class="loginbackground-gridContainer">
          <div
            class="box-root flex-flex"
            style="grid-area: top / start / 8 / end"
          >
            <div
              class="box-root"
              style="
                background-image: linear-gradient(
                  white 0%,
                  rgb(247, 250, 252) 33%
                );
                flex-grow: 1;
              "
            ></div>
          </div>
          <div class="box-root flex-flex" style="grid-area: 4 / 2 / auto / 5">
            <div
              class="box-root box-divider--light-all-2 animationLeftRight tans3s"
              style="flex-grow: 1"
            ></div>
          </div>
          <div
            class="box-root flex-flex"
            style="grid-area: 6 / start / auto / 2"
          >
            <div
              class="box-root box-background--blue800"
              style="flex-grow: 1"
            ></div>
          </div>
          <div
            class="box-root flex-flex"
            style="grid-area: 7 / start / auto / 4"
          >
            <div
              class="box-root box-background--blue animationLeftRight"
              style="flex-grow: 1"
            ></div>
          </div>
          <div class="box-root flex-flex" style="grid-area: 8 / 4 / auto / 6">
            <div
              class="box-root box-background--gray100 animationLeftRight tans3s"
              style="flex-grow: 1"
            ></div>
          </div>
          <div
            class="box-root flex-flex"
            style="grid-area: 2 / 15 / auto / end"
          >
            <div
              class="box-root box-background--cyan200 animationRightLeft tans4s"
              style="flex-grow: 1"
            ></div>
          </div>
          <div
            class="box-root flex-flex"
            style="grid-area: 3 / 14 / auto / end"
          >
            <div
              class="box-root box-background--blue animationRightLeft"
              style="flex-grow: 1"
            ></div>
          </div>
          <div class="box-root flex-flex" style="grid-area: 4 / 17 / auto / 20">
            <div
              class="box-root box-background--gray100 animationRightLeft tans4s"
              style="flex-grow: 1"
            ></div>
          </div>
          <div class="box-root flex-flex" style="grid-area: 5 / 14 / auto / 17">
            <div
              class="box-root box-divider--light-all-2 animationRightLeft tans3s"
              style="flex-grow: 1"
            ></div>
          </div>
        </div>
      </div>
      <div
        class="box-root padding-top--24 flex-flex flex-direction--column"
        style="flex-grow: 1; z-index: 9"
      >
        <div class="formbg-outer">
          <div class="formbg">
            <div class="formbg-inner padding-horizontal--48">
              <form id="stripe-login" @submit.prevent="handleSubmit">
                <div
                  class="box-root padding-top--20 padding-bottom--20 flex-flex flex-justifyContent--center"
                >
                  <h1 class="judul">INPUT DATA</h1>
                </div>
                <div class="field padding-bottom--24">
                  <label for="name">Nama Kapal</label>
                  <input type="text" name="name" v-model="formData.name" />
                </div>
                <div class="field padding-bottom--24">
                  <label for="asal-kapal">Asal Kapal</label>
                  <input
                    type="text"
                    name="asal-kapal"
                    v-model="formData.asalKapal"
                  />
                </div>
                <div class="field padding-bottom--24">
                  <div>
                    <label for="voyage">Tujuan Kapal</label>
                  </div>
                  <input
                    type="text"
                    name="voyage"
                    v-model="formData.tujuanKapal"
                  />
                </div>
                <div class="field padding-bottom--24">
                  <div>
                    <label for="voyage">Nama Muatan</label>
                  </div>
                  <input
                    type="text"
                    name="nama muatan"
                    v-model="formData.namaMuatan"
                  />
                </div>
                <div class="field padding-bottom--24">
                  <input type="submit" value="Submit" />
                </div>
              </form>
              <div v-for="(item, index) in kapalData" :key="index" class="card">
                <div>Nama Kapal: {{ item.name }}</div>
                <div>Asal Kapal: {{ item.asalKapal }}</div>
                <div>Tujuan Kapal: {{ item.tujuanKapal }}</div>
                <div>Nama Muatan: {{ item.namaMuatan }}</div>
                <div>
                  <button class="button-70" @click="editData(index)">
                    Edit
                  </button>
                  <button class="button-80" @click="hapusData(index)">
                    Hapus
                  </button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div> -->
  <!-- <div class="nav w-full flex ">
    <navbar />
  </div> -->
  

  <div class="container">
      <div class="text">
         SEND REQUEST
      </div>
      <form action="#" @submit.prevent="handleSubmit">
         <div class="form-row">
            <div class="input-data">
               <input type="text" required name="name" v-model="formData.name">
               <div class="underline"></div>
               <label for="">Nama Kapal</label>
            </div>
            <div class="input-data">
               <input type="text" required name="asal-kapal"
                    v-model="formData.asalKapal">
               <div class="underline"></div>
               <label for="">Asal Kapal</label>
            </div>
         </div>
         <div class="form-row">
            <div class="input-data">
               <input type="text" required name="voyage"
                    v-model="formData.tujuanKapal">
               <div class="underline"></div>
               <label for="">Tujuan Kapal</label>
            </div>
            <div class="input-data">
               <input type="text" required  name="nama muatan"
                    v-model="formData.namaMuatan">
               <div class="underline"></div>
               <label for="">Nama Muatan</label>
            </div>
         </div>
            
            <div class="form-row submit-btn">
               <div class="input-data">
                  <div class="inner"></div>
                  <input type="submit" value="submit">
               </div>
            </div>   
      </form>
      </div>
<div class="card p-5">
  <div class="text">
         DATA REQUEST
      </div>
      <table class="table mt-5">
  <thead>
    <tr>
      <th>Nama Kapal</th>
      <th>Asal Kapal</th>
      <th>Tujuan Kapal</th>
      <th>Nama Muatan</th>
      <th>Aksi</th>
    </tr>
  </thead>
  <tbody>
    <tr v-for="(item, index) in kapalData" :key="index">
      <td class="bold">{{ item.name }}</td>
      <td>{{ item.asalKapal }}</td>
      <td>{{ item.tujuanKapal }}</td>
      <td>{{ item.namaMuatan }}</td>
      <td>
        <button class="button-70" @click="editData(index)">
          Edit
        </button>
        <button class="button-80" @click="hapusData(index)">
          Hapus
        </button>
      </td>
    </tr>
  </tbody>
</table>
</div>      

</template>

<script>
export default {
  data() {
    return {
      kapalData: [],
      editedIndex: -1,
      editedData: null,
      formData: {
        name: "",
        asalKapal: "",
        tujuanKapal: "",
        namaMuatan: "",
      },
      isEditing: false,
    };
  },
  methods: {
    handleSubmit() {
      console.log("Form submitted");
      const existingDataIndex = this.kapalData.findIndex((item) => {
        return (
          item.name === this.formData.name &&
          item.asalKapal === this.formData.asalKapal &&
          item.tujuanKapal === this.formData.tujuanKapal &&
          item.namaMuatan === this.formData.namaMuatan
        );
      });

      if (this.editedIndex === -1) {
        console.log("Adding new data:", this.formData);
        this.kapalData.push({ ...this.formData });
      } else {
        console.log(
          "Editing data at index",
          this.editedIndex,
          "with new data:",
          this.formData
        );
        this.kapalData[this.editedIndex] = this.formData;
        this.editedIndex = -1;
      }

      this.formData = {
        name: "",
        asalKapal: "",
        tujuanKapal: "",
        namaMuatan: "",
      };
      this.editedData = null;
      this.isEditing = false;
      console.log("Data after submit:", this.kapalData);
    },
    editData(index) {
      this.formData = { ...this.kapalData[index] };
      this.editedIndex = index;
      this.editedData = { ...this.kapalData[index] };
      this.isEditing = true;
    },

    hapusData(index) {
      this.kapalData.splice(index, 1);
    },
  },
};
</script>
