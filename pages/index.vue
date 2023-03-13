<template>
    <div>
        <!--<img src="https://docs.google.com/uc?id=1bfRT8hQhMyGmknQ-S8PHST2CIzf5QmLc" alt="">-->        
        <div class="container-fluid">
        <div class="row">
        </div>
        <!--<section class="vh-600" style="background-color: #508bfc;">-->
        <section class="vh-100" style="background-image: url(https://docs.google.com/uc?id=1bfRT8hQhMyGmknQ-S8PHST2CIzf5QmLc)">
            <div class="container py-5 h-100">
                <div class="row d-flex justify-content-center align-items-center h-100">
                    <div class="col-12 col-md-8 col-lg-6 col-xl-5">
                        <div class="card shadow-2-strong" style="border-radius: 1rem; opacity: 0.9;">
                            <div class="card-body p-5">     
                                <div class="text-center">
                                    <img src="https://docs.google.com/uc?id=1VaNwrme9qpN2u9-PK2mzwklzsW5TC1qy" alt="Bankrut Running" class="brand-image img-circle elevation-3" style="opacity: .8">
                                    <h2>เมนูลงทะเบียน</h2>
                                </div>
                                <form id="account" class="was-validated" novalidate>
                                    <hr />     
                                    <div class="row">
                                        <div class="col-1"></div>
                                        <div class="form-check col-5">
                                        <input class="form-check-input" type="radio" name="flexRadioDefault" id="idSelf" checked>
                                        <label class="form-check-label" for="idSelf">
                                            <h5>ฉันสมัครเอง</h5>
                                        </label>
                                        </div>  
                                        <div class="form-check col-6">
                                        <input class="form-check-input" type="radio" name="flexRadioDefault" id="idFriend">
                                        <label class="form-check-label" for="idFriend">
                                            <h5>สมัครให้เพื่อน</h5>
                                        </label>
                                        </div>            
                                    </div>
                                    <div class="form-floating">
                                        <input type="text" class="form-control" id="floatingNameValue" placeholder="กรุณาป้อนชื่อของท่าน" value="" required>
                                        <label for="floatingNameValue" class="form-label">ชื่อ [ตามหน้าบัตรประจำตัวประชาชน]</label>                                        
                                    </div>
                                    <div class="form-floating">                                        
                                        <input type="text" class="form-control" id="floatingSurnameValue" placeholder="กรุณาป้อนนามสกุล" value="" required>
                                        <label for="floatingSurnameValue">นามสกุล [ตามหน้าบัตรประจำตัวประชาชน]</label>
                                    </div>
                                    <div class="form-floating">                                        
                                        <input type="text" class="form-control" id="floatingPhoneNoValue" placeholder="เบอร์โทรศัพท์ (ที่สามารถติดต่อได้)" value="" required>
                                        <label for="floatingPhoneNoValue">เบอร์โทรศัพท์ [ที่สามารถติดต่อได้]</label>
                                    </div>
                                    <div class="form-floating">                                        
                                        <input type="text" class="form-control" id="floatingEmailValue" placeholder="อีเมล" value="">
                                        <label for="floatingEmailValue">อีเมล </label>
                                    </div>
                                    แนบรูปสลิปการโอนชำระเงิน
                                    <div class="form-floating">
                                        <label for="formFile" class="form-label"></label>
                                        <input class="form-control" type="file" id="formFile">
                                    </div>
                                    <hr/>
                                    <div class="text-center">
                                        <button class="btn btn-lg btn-primary" type="submit">บันทึก</button> |
                                        <button class="btn btn-lg btn-primary" @click="GotoDetail()">รายละเอียด</button>
                                    </div>    
                                </form>                                
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>
    </div>
</template>

<style scope>
img {
    width:35%
}
</style>

<script setup>
    function GotoDetail()
    {        
        navigateTo("/detail")
    }
</script>