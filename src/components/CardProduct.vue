<template>
      <div class="card">
            <p class="discount"><span class="number-discount">-17%</span></p>
            <div class="container-img">
                <img src="../assets/ProductSVG/mango.svg" alt="" class="foods">
            </div>
            <div class="title-rate-price">
                <label for="" class="title">
                    <span class="foodname">Hot pot</span>
                    <span class="description">Seeds of Change Organic Quinoa, Brown, & Red Rice</span>
                </label>
                <div class="star-rate">
                    <div class="stars">
                        <img src="../assets/ProductSVG/start.svg" alt="">
                        <img src="../assets/ProductSVG/start.svg" alt="">
                        <img src="../assets/ProductSVG/start.svg" alt="">
                        <img src="../assets/ProductSVG/start.svg" alt="">
                    </div>
                    <p class="rate">(<span>4.0</span>)</p>
                </div>
                <p class="gram">
                     <span class="number-gram">500</span>
                    <span class="namegram">gram</span>
                </p>
            </div>
            <div class="choose">
                <p class="price">
                    <span class="after-discount-price">$3.5</span>
                    <span class="discount-price">2.00</span>
                </p>
                <div class="input-number">
                    <input type="number" id="number" class="select-number">
                    <div class="arrows">
                        <img src="../assets/svg/upArrow.svg" alt="" class="up">
                        <img src="../assets/svg/downArrow.svg" alt="" class="down">
                    </div>
                </div>
            </div>
        </div>
</template>
<script>

</script>
<style>
.container-product{
                display: flex;
                width: auto;
                gap: 10px;
                flex-wrap: wrap;
}
.discount{
    display: flex;
    width:40px;
    height:23.4px;
    background-color: aqua;
    align-items: center;
    justify-content: center;
    border-radius: 1px 30px 30px 1px;
    position: relative;
    top:14px;
}
.number-discount{
    font-size: 12.6px;
    position: absolute;
}
        .card{
            border: 1px solid rgb(40, 227, 215);
            width:220px;
            border-radius: 10px;
        }
        .stars img{
         width: 12px;
         height: 12px;
        }
        .container-img{
            width:220px;
            display: flex;
            justify-content: center;
            padding-top: 10px;
            padding-bottom: 10px;
        }
       .title .foodname{
            font-size: 12px;
            color: gray;
        }
        .title{
            width: 170px;
            height: auto;
        }
        label{
            margin-bottom:0;
            font-size: 13px;
            display: flex;
            font-family: Georgia, 'Times New Roman', Times, serif;
            flex-direction: column;
        }
        .star-rate{
            display:flex;
            align-content: center;
            gap: 10px;
            }

            .star-rate .stars img {
            width: 12px;
            height: 12px;
            }

            .star-rate p {
            margin: 0;
            font-size: 13px;
            color: #333;
            }
            p,.rate{
            display: inline; 
            }

            .gram {
                display: flex;
                align-content: center;
                flex-direction: row;
                gap: 10px;
                margin-bottom: 0;
            }

            .select-number {
            width: 65px;
            height: 27px;
            font-size: 14px;
            border: 2px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box;
            transition: border-color 0.3s;
            position: relative;
            color:rgb(95, 201, 95);
        }
    
        .select-number::-webkit-inner-spin-button,
        .select-number::-webkit-outer-spin-button {
            -webkit-appearance: none;
        }
     .gram{
        font-family: 'Lucida Sans';
        font-size: 17px;
     }
        .select-number:focus {
            border-color: rgb(102, 236, 189);
            outline: none;
        }

        .select-number {
            border-color: rgb(70, 229, 173);
            padding-left: 7px;
        }

        .down,
        .up {
            width: 7px;
            cursor: pointer;
            padding-right: 5px;
        }

        .arrows {
            display: flex;
            flex-direction: column;
            gap: 3px;
        }

        .input-number {
            position: relative;
            background-color: rgb(41, 119, 188);
            border-radius: 10px;
            border: 1px;
        }
        .discount-price{
            text-decoration:line-through gray;
            font-size: 16px;

        }
        .after-discount-price{
                font-size: 18px;
        }
        .price{
            display: flex;
            gap:10px;
            flex-direction: row;
            justify-content: center;
            align-content: center;
            padding-top: 13px;
            padding-bottom: 0;
        }
        .arrows {
            position: absolute;
            right: 4px;
            top: 0;
            bottom: 0;
            display: flex;
            flex-direction: column;
            justify-content: center;
            gap: 2px;
        }
        .choose{
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding-left: 10px;
            padding-bottom: 14px;
            padding-right: 10px;
        }
        .title-rate-price{
        padding-left: 10px;
        }
</style>