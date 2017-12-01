<style scoped>
a:hover, a:visited, a:link, a:active {
    text-decoration: none;
    color: #eee;
}
a:active,a:hover{
    color: #fff;
}
.layout{
    background: #ecf0f1;
}
.top-bar{
    width: 100%;
    height: 80px;
    position:fixed;
    top:0;
    z-index: 1;
}
.layout-topbar-wrapper{
    width: 1170px;
    height: 100%;
    position: relative;
    margin: 0 auto;
}
.layout-logo{
    width: 100px;
    height: 100%;
    line-height: 80px;
    position: absolute;
    color:#ffffff;
    left: 20px;
}
.layout-nav{
    width: 525px;
    height: 100%;
    line-height: 80px;
    position: absolute;
    right: 0;
}
.layout-nav li{
    height: 100%;
    line-height: 80px;
}
.group-wrapper{
    width: 100%;
}
.group-wrapper-home{
    width: 100%;
    height: 850px;
}
.group{
    width: 1140px;
    height: 100%;
    position: relative;
    margin: 0 auto;
    color: #ffffff;
}
.menu-back{
    background-color: #3498db;
}
.home-back{
    background-color: #3498db;
}
.people-back{
    background-color: #ecf0f1;
}
.publication-back{
    background-color: #27ae60;
}
.project-back{
    background-color: #ecf0f1;
}
.contact-back{
    background-color: #ecf0f1;
}
.home-font{
    position: relative;
    margin: 0 auto;
    text-align: center;
}
.font1{
    padding: 320px 0 48px;
    font: bold 86px "Raleway";
    color:#ecf0f1;
}
.font2{
    font: bold 60px "Raleway";
    color:#ecf0f1;
}
.home-details{
    width:1140px;
    height:580px;
    position:absolute;
    bottom: -380px;
    padding:70px 0;
    background-color: #ffffff;
    border-bottom: 2px solid #d0d4d4;
    border-right: 2px solid #d0d4d4;
    border-radius: 3px;
    color:#2c3e50;
}
.font-title{
    font: normal 40px "Raleway";
}
.font-subtitle{
    margin: 42px 0 72px;
    font: normal 20px "Raleway";
}
.font-p{
    font: normal 20px "Raleway";
}
.home-details h3{
    width: 100%;
    margin-bottom: 100px;
    text-align: center;
}
.home-details p{
    width: 770px;
    margin: 10px auto;
}
.group-people{
    margin-top: 470px;
}
.title-a{
    text-align: center;
    color:#2c3e50;
}
.title-b{
    text-align: center;
    color:#ffffff;
}
.people-details{
    margin-bottom: 100px;
    font: 20px "Raleway";
    color:#2c3e50;
}
.publication-list{
    margin: 0 30px;
    list-style-type: disc;
}
.project-carousel{
    display: flex;
    align-items: center;
    width: 100%;
    height: 300px;
    text-align: center;
    background-color: #2c3e50;
    font: 30px "Raleway";
}
.demo-carousel{
    flex: 1;
    justify-content: center;
}
.contact-font{
    color:#2c3e50;
    font: 18px "Raleway";
}
.contact-font *{
    text-align: center;
}
.hr-footer{
    width: 400px;
    margin: 20px auto;
    font-size: small;
    color:#eeeeee;
}
footer{
    text-align: center;
    color:#2c3e50;
    font: 18px "Raleway";
}
</style>
<template>
     <div class="layout">
        <BackTop></BackTop>
        <Menu mode="horizontal" theme="dark" active-name="1" class="menu-back top-bar" id="home">
            <div class="layout-topbar-wrapper">
            <div class="layout-logo">SQUARE</div>
            <div class="layout-nav">
                <MenuItem name="1">
                    <a href="#home">Home</a>
                </MenuItem>
                <MenuItem name="2">
                    <a href="#people">People</a>
                </MenuItem>
                <MenuItem name="3">
                    <a href="#publication">Publication</a>
                </MenuItem>
                <MenuItem name="4">
                    <a href="#project">Project</a>
                </MenuItem>
                <MenuItem name="5">
                    <a href="#contact">Contact</a>
                </MenuItem>
            </div>
            </div>
        </Menu>
        <div class="group-wrapper-home home-back">
        <div class="group group-home">
            <div class="font1 home-font">HELLO!</div>
            <div class="font2 home-font">WE ARE SQUARE</div>
            <div class="home-details">
                <h3 class="font-title">ABOUT US</h3>
                <p class="font-p">constructing......</p>
            </div>
        </div>
        </div>
        <div class="group-wrapper people-back" id="people">
        <div class="group group-people">
        <Row class="title-a font-title">OUR TEAM</Row>
        <Row class="title-a font-subtitle">brief......</Row>
        <Row :gutter="16" class="people-details font-p">
        <Col span="12">
            <Collapse accordion>
                <Panel name="1">
                     Professor
                    <p slot="content">史蒂夫·乔布斯（Steve Jobs），1955年2月24日生于美国加利福尼亚州旧金山，美国发明家、企业家、美国苹果公司联合创办人。</p>
                </Panel>
                <Panel name="2">
                     Senior Engineer
                    <p slot="content">史蒂夫·乔布斯（Steve Jobs），1955年2月24日生于美国加利福尼亚州旧金山，美国发明家、企业家、美国苹果公司联合创办人。</p>
                </Panel>
                <Panel name="3">
                     Lecture
                    <p slot="content">史蒂夫·乔布斯（Steve Jobs），1955年2月24日生于美国加利福尼亚州旧金山，美国发明家、企业家、美国苹果公司联合创办人。</p>
                </Panel>
            </Collapse>
        </Col>
        <Col span="12">
            <Collapse accordion>
                <Panel name="1">
                     Ph.D. Student
                    <p slot="content">史蒂夫·乔布斯（Steve Jobs），1955年2月24日生于美国加利福尼亚州旧金山，美国发明家、企业家、美国苹果公司联合创办人。</p>
                </Panel>
                <Panel name="2">
                     Master Student
                    <p slot="content">史蒂夫·乔布斯（Steve Jobs），1955年2月24日生于美国加利福尼亚州旧金山，美国发明家、企业家、美国苹果公司联合创办人。</p>
                </Panel>
                <Panel name="3">
                     Graduated Student
                    <p slot="content">史蒂夫·乔布斯（Steve Jobs），1955年2月24日生于美国加利福尼亚州旧金山，美国发明家、企业家、美国苹果公司联合创办人。</p>
                </Panel>
            </Collapse>
        </Col>
        </Row>
        </div>
        </div>
        <div class="group-wrapper publication-back" id="publication">
        <div class="group group-publication">
        <Row class="title-b font-title">Publication</Row>
        <ul class="publication-list font-p">
            <li>aaa</li>
            <li>bbb</li>
            <li>ccc</li>
        </ul>
        </div>
        </div>
        <div class="group-wrapper project-back" id="project">
        <div class="group group-project">
        <Row class="title-a font-title">Project</Row>
        <Carousel autoplay loop class="project-carousel">
        <CarouselItem>
            <div class="demo-carousel">1</div>
        </CarouselItem>
        <CarouselItem>
            <div class="demo-carousel">2</div>
        </CarouselItem>
        <CarouselItem>
            <div class="demo-carousel">3</div>
        </CarouselItem>
        <CarouselItem>
            <div class="demo-carousel">4</div>
        </CarouselItem>
        </Carousel>
        </div>
        </div>
        <div class="group-wrapper" id="contact">
        <div class="group contact-font">
        <Row class="title-a font-title">Contact Us</Row>
        <h4>name</h4>
        <p>sub-title</p>
        <p>abstract</p>
        <ul>
            <li>address</li>
            <li>tel</li>
            <li>email</li>
        </ul>
        </div>
        </div>
        <div class="group">
        <hr class="hr-footer">
        <footer>Copyright</footer>
        </div>
     </div>
</template>
<script>
    export default {
    }
</script>
