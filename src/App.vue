<script>
export default {
  data() {
    return {  
      picked: {
        iam:"",
        Name:"",
        Lname:"",
        ID:"",
        Major:"",
        Group:"",
        Course:"",
        Subject:"",
        Day:"",
        Time:"",
        Test:"",
        Daytime:"",
        Text:""
      } 
  
  };
  },
};
</script>
<template>
  <div class="container">
    <div class="row text-center">
      <div>
        <h1>คำร้องขอเลื่อนสอบเเละสอบชดใช้</h1>
        <br />
      </div>
    </div>
    <div class="row">
      <div class="d-flex justify-content-center">
        <form action="">
          <div class="d-flex justify-content-end"><input type="date" /></div>
          <br />
          ข้าพเจ้า
          <select name="" id="" v-model="picked.iam">
            <option value="นาย">นาย</option>
            <option value="นาง">นาง</option>
            <option value="นางสาว">นางสาว</option>
          </select>
          ชื่อ
          <input type="text" v-model="picked.Name"/>
          นามสกุล
          <input type="text" v-model="picked.Lname" /><br />
          รหัสนักศึกษา
          <input type="text" v-model="picked.ID"/>
          สาขาวิชา
          <select name="selectgrop" v-model="picked.Group">
          <option value="คณะผลิตกรรมการเกษตร">คณะผลิตกรรมการเกษตร</option>
          <option value="คณะบริหารธุรกิจ">คณะบริหารธุรกิจ</option>
          <option value="คณะวิทยาศาสตร์">คณะวิทยาศาสตร์</option>
          <option value="คณะศิลปศาสตร์">คณะศิลปศาสตร์</option>
          <option value="คณะสถาปัตยกรรมศาสตร์ และการออกแบบสิ่งแวดล้อม ">
            คณะสถาปัตยกรรมศาสตร์ และการออกแบบสิ่งแวดล้อม
          </option>
          <option value="คณะเทคโนโลยีการประมง และทรัพยากรทางน้ำ">
            คณะเทคโนโลยีการประมง และทรัพยากรทางน้ำ
          </option>
          <option value="คณะวิศวกรรมและอุตสาหกรรมเกษตร ">
            คณะวิศวกรรมและอุตสาหกรรมเกษตร
          </option>
          <option value="คณะพัฒนาการท่องเที่ยว ">คณะพัฒนาการท่องเที่ยว</option>
          <option value="คณะเศรษฐศาสตร์ ">คณะเศรษฐศาสตร์</option>
          <option value="วิทยาลัยบริหารศาสตร์ ">วิทยาลัยบริหารศาสตร์</option>
          <option value="วิทยาลัยพลังงานทดแทน ">วิทยาลัยพลังงานทดแทน</option>
          <option value="วิทยาลัยนานาชาติ ">วิทยาลัยนานาชาติ</option>
          <option value="มหาวิทยาลัยแม่โจ้-แพร่ เฉลิมพระเกียรติ ">
            มหาวิทยาลัยแม่โจ้-แพร่ เฉลิมพระเกียรติ
          </option>
          <option value="มหาวิทยาลัยแม่โจ้-ชุมพร ">มหาวิทยาลัยแม่โจ้-ชุมพร</option>
          <option value="คณะพยาบาลศาสตร์">คณะพยาบาลศาสตร์</option>
          <option value="คณะสัตวแพทย์ศาสตร์">คณะสัตวแพทย์ศาสตร์</option>
        </select><br>
          คณะ
          <select name="" id="" v-model="picked.Group">
            <option value="คณะผลิตกรรมการเกษตร">คณะผลิตกรรมการเกษตร</option>
            <option value="คณะวิศวกรรมเเละอุตสาหกรรม">คณะวิศวกรรมเเละอุตสาหกรรม</option>
            <option value="คณะวิทยาศาสตร์">คณะวิทยาศาสตร์</option>
            <option value="คณะวิทยาลัยบริหารศาสตร์">คณะวิทยาลัยบริหารศาสตร์</option>
            <option value="คณะบริหารธุรกิจ">คณะบริหารธุรกิจ</option>
            <option value="คณะพัฒนาการท่องเที่ยว">คณะพัฒนาการท่องเที่ยว</option>
            <option value="คณะเทคโนโลยีการประมงเเละทรัพยากรทางน้ำ">
              คณะเทคโนโลยีการประมงเเละทรัพยากรทางน้ำ
            </option>
            <option value="คณะเศรษฐศาสตร์">คณะเศรษฐศาสตร์</option>
            <option value="คณะศิลปศาสตร์">คณะศิลปศาสตร์</option>
            <option value="คณะวิทยาลัยพลังงานทดเเทน">คณะวิทยาลัยพลังงานทดเเทน</option>
            <option value="คณะสารสนเทศเเละการสื่อสาร">คณะสารสนเทศเเละการสื่อสาร</option>
            <option value="คณะสถาปัตยกรรมศาสตร์เเละการออกเเบบสิ่งเเวดล้อม">
              คณะสถาปัตยกรรมศาสตร์เเละการออกเเบบสิ่งเเวดล้อม
            </option>
            <option value="คณะสัตวศาสตร์เเละเทคโนโลยี">คณะสัตวศาสตร์เเละเทคโนโลยี</option>
            <option value="มหาวิทยาลัยเเม่โจ้-เเพร่ เฉลิมพระเกีตรติ">
              มหาวิทยาลัยเเม่โจ้-เเพร่ เฉลิมพระเกีตรติ
            </option>
            <option value="มหาวิทยาลัยเเม่โจ้-ชุมพร">
              มหาวิทยาลัยเเม่โจ้-ชุมพร
            </option></select
          ><br />
          หลักสูตร ปริญญาตรี
          <input type="radio" name="4-5ปี" id="" value="4-5ปี" v-model="picked.Course">
          4-5ปี
          <input type="radio" name="4 ปีเทียบเข้าเรียปีน(2)" id="" value="4 ปีเทียบเข้าเรียปีน(2)" v-model="picked.Course">
          4 ปีเทียบเข้าเรียน(2ปี)<br>
          มีความประสงค์ขอเลื่อนสอบ รายวิชา
          <input type="text" v-model="picked.Test" /><br />
          ใน เดือน/วัน/ปี
          <input type="date" name="" id="" v-model="picked.Day"/>
          ในเวลา
          <input type="time" name="" id="" v-model="picked.Time"/><br />
          เนื่องจาก
          <input type="text" size="100" v-model="picked.Text"/><br />
          ทั้งนี้จะขอสอบชดใข้ ในวันที่
          <input type="datetime-local" name="" id="" v-model="picked.Daytime"/><br />
          จึงเรียนมาเพื่อโปรดพิจารณา
        </form>
      </div>
    </div>
  </div>
  <h5 class="justify-content-top">{{ picked }}</h5><br>
</template>
<style></style>
