<template>
    <div>             
        <!--<img src="https://docs.google.com/uc?id=1bfRT8hQhMyGmknQ-S8PHST2CIzf5QmLc" alt="">-->        
        <div class="container-fluid">
        <div class="row">
        </div>
        <section class="vh-600" style="background-color: #508bfc;">
            <div class="container py-5 h-100">
                <div class="row d-flex justify-content-center align-items-center h-100">
                    <div class="col-12 col-md-8 col-lg-6 col-xl-5">
                        <div class="card shadow-2-strong" style="border-radius: 1rem;">
                            <div class="card-body p-5 text-center">                                
                                <img src="https://docs.google.com/uc?id=1VaNwrme9qpN2u9-PK2mzwklzsW5TC1qy" alt="Bankrut Running" class="brand-image img-circle elevation-3" style="opacity: .8">
                                <h2>กรุณากรองข้อมูลด้านล่างนี้</h2>
                                <form id="account" method="post">
                                    <hr />                 
                                    <div class="form-floating">
                                        <input type="name" class="form-control" id="floatingNameValue" placeholder="" value="">
                                        <label for="floatingNameValue">กรุณาป้อนชื่อ</label>                                                                                
                                    </div>
                                    <div class="form-floating">                                        
                                        <input type="name" class="form-control" id="floatingSurnameValue" placeholder="" value="">
                                        <label for="floatingSurnameValue">กรุณาป้อนนามสกุล</label>
                                    </div>
                                    <div class="form-floating">                                        
                                        <input type="name" class="form-control" id="floatingPhoneNoValue" placeholder="" value="">
                                        <label for="floatingPhoneNoValue">เบอร์โทรศัพท์(ที่สามารถติดต่อได้)</label>
                                    </div>
                                    <br/>
                                    <div>                                        
                                        <button class="btn btn-primary" type="submit">บันทึก</button> |
                                        <button type="button" class="btn btn-secondary" @click="CloseWindow();">ยกเลิก</button>
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

<script setup>
    function CloseWindow() {
        window.close();
    }

</script>

<style scope>
img {
    width:50%
}
</style>