<template>
<div class="sidebar-container">
  <div class="sidebar">
    <!-- شعار المركبة -->
    <img src="@/assets/مركبة.svg" alt="Logo" class="logo" />

    <!-- قائمة التنقل -->
    <ul class="nav">
      
      <!-- عنصر لوحة التحكم -->
      <li class="nav-item">
        <a class="nav-link active text-light" href="#" style="font-size: 14px; border-radius: 15px; background-color: #635BFF;">
          <img src="@/assets/dash.svg" class="me-1" /> Dashboard
        </a>
      </li>

      <!-- عنصر الطلبات -->
      <li class="nav-item">
        <router-link to="/orders" class="nav-link text-dark">
          <img :src="require('@/assets/OR.svg')" alt="Orders" class="icon" />
          Orders
        </router-link>
      </li>

      <!-- عنصر الركاب -->
      <li class="nav-item">
        <router-link to="/passengers" class="nav-link text-dark">
          <img :src="require('@/assets/PASS.svg')" alt="Passengers" class="icon" />
          Passengers
        </router-link>
      </li>

      <!-- عنصر الكابتن -->
      <li class="nav-item">
        <router-link to="/captains" class="nav-link text-dark">
          <img :src="require('@/assets/CAPT.svg')" alt="Captains" class="icon" />
          Captains
        </router-link>
      </li>

      <!-- عنصر الفئات -->
      <li class="nav-item">
        <router-link to="/categories" class="nav-link text-dark">
          <img :src="require('@/assets/CAT.svg')" alt="Categories" class="icon" />
          Categories
        </router-link>
        <hr />
      </li>

      <!-- عنصر التسوية -->
      <li class="nav-item">
        <router-link to="/settlement" class="nav-link text-dark">
          <img :src="require('@/assets/SETT.svg')" alt="Settlement" class="icon" />
          Settlement
        </router-link>
        <hr />
      </li>

      <!-- عنصر الاتصال -->
      <li class="nav-item">
        <router-link to="/contact" class="nav-link text-dark">
          <img :src="require('@/assets/CONTA.svg')" alt="Contact" class="icon" />
          Contact
        </router-link>
      </li>

      <!-- عنصر المراجعات -->
      <li class="nav-item">
        <router-link to="/reviews" class="nav-link text-dark">
          <img :src="require('@/assets/RERE.svg')" alt="Reviews" class="icon" />
          Reviews
        </router-link>
        <hr />
      </li>

      <!-- عنصر الصلاحيات مع قائمة منسدلة -->
      <li class="nav-item dropdown">
        <a class="nav-link text-dark dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown">
          <img :src="require('@/assets/PERM.svg')" alt="Permissions" class="icon" />
          Permissions
        </a>
        <div class="nav-item">
          <router-link to="/translation" class="nav-link text-dark">
            <img :src="require('@/assets/transla.svg')" alt="Translation" class="icon" />
            Translation
          </router-link>
          <router-link to="/education-video" class="nav-link text-dark">
            <img :src="require('@/assets/EDU.svg')" alt="Education Video" class="icon" />
            Education Video
          </router-link>
        </div>
      </li>

      <!-- عنصر الإعدادات -->
      <li class="nav-item">
        <router-link to="/settings" class="nav-link text-dark">
          <img :src="require('@/assets/SETTIN.svg')" alt="Settings" class="icon" />
          Settings
        </router-link>
      </li>

      <!-- عنصر المحتوى -->
      <li class="nav-item">
        <router-link to="/content" class="nav-link text-dark">
          <img :src="require('@/assets/COCOCO.svg')" alt="Content" class="icon" />
          Content
        </router-link>
      </li>
      
    </ul>
  </div>
</div>

<!-- الهيدر الأول -->
<header class="header d-flex justify-content-between align-items-center p-3 bg-light border-bottom" style="margin-left: 220px;">
  <div class="d-flex align-items-center">
    <!-- زر البحث -->
    <button class="btn btn-icon">
      <img :src="require('@/assets/SEARCH.svg')" alt="Search" />
    </button>
    <!-- زر الشبكة -->
    <button class="btn btn-icon">
      <img :src="require('@/assets/GRID.svg')" alt="Grid" />
    </button>
  </div>

  <div class="d-flex align-items-center">
    <!-- أيقونة المراقبة -->
    <button class="btn btn-icon">
      <img :src="require('@/assets/mon.svg')" alt="Monitor" />
    </button>
    <!-- أيقونة التشغيل -->
    <button class="btn btn-icon">
      <img :src="require('@/assets/runrun.svg')" alt="Run" />
    </button>
    <!-- أيقونة اللغة -->
    <button class="btn btn-icon">
      <img :src="require('@/assets/ENG.svg')" alt="Language" />
    </button>

    <!-- قائمة المستخدم -->
    <div class="user-dropdown d-flex align-items-center">
      <button class="btn btn-icon user">
        <img :src="require('@/assets/USER.svg')" alt="User" />
      </button>
      <!-- سهم القائمة المنسدلة -->
      <button class="btn btn-icon">
        <i class="bi bi-chevron-down"></i>
      </button>
    </div>
  </div>
</header>

<!-- الهيدر الثاني -->
<div class="p-3 bg-light border-bottom header-2" style="margin-left: 220px; margin-top: 10px;">
  <div class="d-flex justify-content-between align-items-center">
    <!-- عنوان الهيدر الثاني -->
    <h5 class="mb-0">Chat</h5>
    <!-- الأيقونات الخاصة بالشات -->
    <div class="d-flex align-items-center">
      <img :src="require('@/assets/SWEEET.svg')" class="me-2" alt="Sweet" />
      <img :src="require('@/assets/QQQ.svg')" class="me-2" alt="QQQ" />
      <!-- شارة المحادثة -->
      <span class="badge custom-badge">Chat</span>
    </div>
  </div>
</div>
    <!-- نافذة الدردشة -->
    <div class="container mt-4 ">
      <div class="row justify-content-end ms-4">
    <!-- القسم الأول - Profile (4 columns) -->
    <div class="col-3 p-0">
      <div class="card m-0 h-100">
        <div class="actions">
            <div class="chat">
            <div class="card-body">
              <div>
    <!-- User Profile Section -->
    <div class="user-profile d-flex align-items-center mb-3">
  <img src="@/assets/Mathew Anderson.svg" alt="Profile picture" class="me-3 rounded-circle" style="width: 54px; height: 54px;">
  <!-- اسم المستخدم والوظيفة -->
  <div class="ms-3 flex-grow-1">
    <h2 style="font-size: 15px;">Mathew Anderson</h2>
    <p class="mb-0 text-muted" style="font-size: 12px;">Marketing Director</p>
  </div>
  <!-- ثلاث نقاط على اليمين بعد الاسم -->
  <div class="d-flex align-items-center">
    <span class="status-dot bg-success rounded-circle me-2"></span>
    <i class="bi bi-three-dots-vertical"></i> <!-- ثلاث نقاط فوق بعضها -->
  </div>
</div>
</div>
<!-- Search Bar Section -->
<div class="search-bar p-3 border-bottom d-flex align-items-center">
  <div class="input-group">
    <!-- أيقونة البحث داخل المربع على اليسار -->
    <span class="input-group-text bg-white border-end-0">
      <i class="bi bi-search"></i> <!-- أيقونة البحث -->
    </span>
    <!-- مربع البحث -->
    <input type="text" class="form-control border-start-0" placeholder="Search contacts" />
  </div>
</div>
   <!-- Dropdown Section -->
<div class="dropdown mt-3">
    <button class="btn text-secondary dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false" style="font-size: 14px;">
        Recent chats
    </button>
</div>
<ul class="recent-chats list-unstyled mt-3">
    <!-- First Chat Item -->
    <li class="list-group-item d-flex align-items-center mb-3" style="background-color: #F6F7F9; border-radius: 8px;">
          <img src="@/assets/Mioff.svg" alt="Profile" class="me-3 rounded-circle" width="48" height="48">
          <div class="chat-info flex-grow-1">
            <h3 class="mb-0" style="font-size: 15px;">Michell Flintoff</h3>
            <small class="text-muted">You: Yesterdy was great...</small>
        </div>
        <small class="text-muted">15 minutes</small>
    </li>
    <!-- Second Chat Item -->
    <li class="list-group-item d-flex align-items-center mb-3">
        <img src="@/assets/Bi.svg" alt="Profile" width="48" height="48">
        <div class="chat-info flex-grow-1">
            <h3 class="mb-0" style="font-size: 15px;">Bianca Anderson</h3>
            <small class="text-muted">Nice looking dress you...</small>
        </div>
        <small class="text-muted">30 minutes</small>
    </li>
    <!-- Third Chat Item -->
    <li class="list-group-item d-flex align-items-center mb-3">
        <img src="@/assets/Andrew.svg" alt="Profile" class="me-3 rounded-circle" width="48" height="48">
        <div class="chat-info flex-grow-1">
            <h3 class="mb-0" style="font-size: 15px;">Andrew Johnson</h3>
            <small class="text-muted">Sent a photo</small>
        </div>
        <small class="text-muted">2 hours</small>
    </li>
    <!-- Fourth Chat Item -->
    <li class="list-group-item d-flex align-items-center mb-3">
        <img src="@/assets/Mark1.svg" alt="Profile" class="me-3 rounded-circle" width="48" height="48">
        <div class="chat-info flex-grow-1">
            <h3 class="mb-0" style="font-size: 15px;">Mark Strokes</h3>
            <small class="text-muted">Lorem ispusm text sud...</small>
        </div>
        <small class="text-muted">5 days</small>
    </li>
    <!-- Fifth Chat Item -->
    <li class="list-group-item d-flex align-items-center mb-3">
        <img src="@/assets/MarkST.svg" alt="Profile" class="me-3 rounded-circle" width="48" height="48">
        <div class="chat-info flex-grow-1">
            <h3 class="mb-0" style="font-size: 15px;">Mark, Stoinus & Rish...</h3>
            <small class="text-muted">Lorem ispusm text ...</small>
        </div>
        <small class="text-muted">5 days</small>
    </li>
    <!-- Sixth Chat Item -->
    <li class="list-group-item d-flex align-items-center mb-3">
        <img src="@/assets/Bi.svg" alt="Profile" class="me-3 rounded-circle" width="48" height="48">
        <div class="chat-info flex-grow-1">
            <h3 class="mb-0" style="font-size: 15px;">Bianca Anderson</h3>
            <small class="text-muted">Nice looking dress you...</small>
        </div>
        <small class="text-muted">30 minutes</small>
    </li>
</ul>
 </div>
          </div>
        </div>
      </div>
    </div>
    <!-- القسم الثاني - Chat (5 columns) -->
    <div class="col-md-5 p-0">
      <div class="card m-0 h-100">
        <div class="card-body">
          <div class="d-flex align-items-center mb-3">
            <img src="@/assets/AWAY.svg" class="me-1" />
            <div class="ms-3">
              <small class="text-muted">Away</small>
            </div>
          </div>
          <hr>
           <!-- Dialog -->
<div v-if="showDialog" class="dialog-overlay" @click="closeDialog">
      <div class="dialog-content" @click.stop>
        <div class="dialog-header">
          <img :src="dialogIcon"  class="dialog-icon" />
          <h3 class="dialog-title">{{ dialogTitle }}</h3>
        </div>
        <p class="dialog-message">{{ dialogMessage }}</p>
        <div class="dialog-actions">
          <button class="btn-cancel" @click="closeDialog">Cancel</button>
          <button class="btn-confirm" @click="confirmAction">Yes</button>
        </div>
      </div>
    </div>
    <div class="chat-messages mb-3 flex-grow-1" style="overflow-y: auto;">
            <div class="d-flex mb-3">
              <img src="@/assets/AND2.svg" class="me-1" />
              <div class="ms-3">
                <small class="text-muted"  style=" font-size: 12px;">Andrew, 2 hours ago</small>
                <p class="bg-light p-2 rounded ">If I don't like something, I'll stay away from it.</p>
              </div>
            </div>
            <div class="d-flex justify-content- mb-3">
              <div class="ms-3">
                <small class="text-muted"  style=" font-size: 12px;">2 hours ago</small>
                <p class="text-dark p-2 rounded" style="background-color: #ECFDFD;" >If I don't like something, I'll stay away from it.</p>
              </div>
            </div>
            <div class="d-flex mb-3">
              <img src="@/assets/AND2.svg" class="me-1" />
              <div class="ms-3">
                <small class="text-muted"  style=" font-size: 12px;">Andrew, 2 hours ago</small>
                <p class="bg-light p-2 rounded">I want more detailed information.</p>
              </div>
            </div>
            <div class="d-flex justify-content-end mb-3">
              <div class="ms-3">
                <small class="text-muted" style=" font-size: 12px;">2 hours ago</small>
                <p class="text-dark p-2 rounded" style="background-color: #ECFDFD;" >If I don’t like something, I’ll stay away from it.</p>
                <p class="text-dark p-2 rounded" style="background-color: #ECFDFD;" >They got there early, and they got really good seats.</p>
              </div>
            </div>

            <div class="d-flex flex-column mb-3">
              <div class="d-flex align-items-center">
                <!-- صورة الشخص -->
                 <img src="@/assets/AND2.svg" class="me-2" style="width: 40px; height: 40px;" />
                 <!-- اسم الشخص ووقت الإرسال بجانب الصورة -->
                  <div class="d-flex flex-column">
                    <small style="font-size: 14px;">Andrew</small>
                    <small class="text-muted" style="font-size: 12px;">2 hours ago</small>
                  </div>
                </div>
         <!-- الصورة المرسلة تبدأ مباشرة أسفل الاسم والوقت -->
        <div class="d-flex justify-content-start mt-2">
        <img src="@/assets/mac.svg"/>
        </div>
        </div>
       
        <div class="message-bar d-flex align-items-center p-2">  
          <!-- Emoji Icon -->
        <i class="bi bi-emoji-smile fs-3 me-2"></i>
         <!-- Text Input -->
        <input
               type="text"
                    class="form-control message-input flex-grow-1"
                          placeholder="Type a Message"/>
    <!-- Icons -->
    <img src="@/assets/iimage.svg"/>
    <img src="@/assets/clip.svg"/>
    <img src="@/assets/maic.svg"/>
  </div>
 </div>          
 </div>
</div>
</div>
    <!-- القسم الثالث - Files & Media (3 columns) -->
<div class="col-md-3 p-0">
  <div class="card m-0 h-100">
    <div class="card-body">
      <div class="d-flex align-items-center">
      <a href="#" class="icon2" @click="openDialog('rcan1')">
        <img src="@/assets/rcan1.svg" class="me-1" alt="Block" />
      </a>
      <a href="#" class="icon2" @click="openDialog('newdlet')">
        <img src="@/assets/newdlet.svg" class="me-1" alt="Delete" />
      </a>
      <a href="#" class="icon2" @click="openDialog('unlock')">
        <img src="@/assets/unlock.svg" class="me-1" alt="unlock" />
      </a>
      <a href="#" class="icon2" >
        <img src="@/assets/CALL.svg" class="me-1" alt="Clip" />
      </a >
      <a  href="#" class="icon2">
        <img src="@/assets/VEDU.svg" class="me-1" alt="tele" />
      </a>
      <a  href="#" class="icon2">
        <img src="@/assets/MORE.svg" class="me-1" alt="slid" />
      </a>
    </div>
<br/>
<hr>
          <!-- قسم الوسائط -->
<div class="media-section mb-4">
<h5 style="font-size: 15px;"> Media <span style="color: #98A4AE;">(36)</span></h5>
<div class="row">
<div class="row">
<div class="col-4 p-1">
<img :src="require('@/assets/medo1.svg')" class="media-icon" alt="media" />
</div>
<div class="col-4 p-1">
<img :src="require('@/assets/medo2.svg')" class="media-icon" alt="media" />
</div>
<div class="col-4 p-1">
 <img :src="require('@/assets/medo3.svg')" class="media-icon" alt="media" />
   </div>
  </div>

<div class="row">
  <div class="col-4 p-1">
    <img :src="require('@/assets/medo4.svg')" class="media-icon" alt="media" />
  </div>
  <div class="col-4 p-1">
    <img :src="require('@/assets/medo1.svg')" class="media-icon" alt="media" />
  </div>
  <div class="col-4 p-1">
    <img :src="require('@/assets/medo2.svg')" class="media-icon" alt="media" />
  </div>
</div>
</div>
</div>
         <!-- قسم الملفات -->
<div class="files-section">
<h5 style="font-size: 15px;"> Files <span style="color: #98A4AE;">(36)</span></h5>
<ul class="list-group">
<li class="list-group-item d-flex align-items-center small" style="border: none;">
            <!-- صورة على اليسار -->
            <img :src="require('@/assets/SERV.svg')" class="media-icon me-3" />
            <!-- نص بجانب الصورة -->
            <div class="d-flex flex-column">
              <!-- اسم الملف -->
              <span class="text-truncate" style="font-size: 15px;">server-task.pdf</span>
              <!-- توقيت أسفل اسم الملف -->
              <small class="text-muted" style="font-size: 12px;">2 MB 2 Dec 2022</small>
            </div>
            <!-- حجم الملف في نهاية العنصر -->
            <small class="ms-auto text-muted" style="font-size: 12px;"></small>
          </li>
          <li class="list-group-item d-flex align-items-center small" style="border: none;">
            <!-- صورة على اليسار -->
            <img :src="require('@/assets/home.svg')" class="media-icon me-3" alt="pdf" />
            <!-- نص بجانب الصورة -->
            <div class="d-flex flex-column">
              <!-- اسم الملف -->
              <span class="text-truncate" style="font-size: 15px;">homepage-design.fig</span>
              <!-- توقيت أسفل اسم الملف -->
              <small class="text-muted" style="font-size: 12px;">2 MB 2 Dec 2022</small>
            </div>
            <!-- حجم الملف في نهاية العنصر -->
            <small class="ms-auto text-muted" style="font-size: 12px;"></small>
          </li>
          <li class="list-group-item d-flex align-items-center small" style="border: none;">
            <!-- صورة على اليسار -->
            <img :src="require('@/assets/sbout.svg')" class="media-icon me-3" />
            <!-- نص بجانب الصورة -->
            <div class="d-flex flex-column">
              <!-- اسم الملف -->
              <span class="text-truncate" style="font-size: 15px;">about-us.html</span>
              <!-- توقيت أسفل اسم الملف -->
              <small class="text-muted" style="font-size: 12px;">2 MB 2 Dec 2022</small>
            </div>
            <!-- حجم الملف في نهاية العنصر -->
            <small class="ms-auto text-muted" style="font-size: 12px;"></small>
          </li>
          <li class="list-group-item d-flex align-items-center small" style="border: none;">
            <!-- صورة على اليسار -->
            <img :src="require('@/assets/workht.svg')" class="media-icon me-3" />
            <!-- نص بجانب الصورة -->
            <div class="d-flex flex-column">
              <!-- اسم الملف -->
              <span class="text-truncate" style="font-size: 15px;">work-project.zip</span>
              <!-- توقيت أسفل اسم الملف -->
              <small class="text-muted" style="font-size: 12px;">2 MB 2 Dec 2022</small>
            </div>
            <!-- حجم الملف في نهاية العنصر -->
            <small class="ms-auto text-muted" style="font-size: 12px;"></small>
          </li>
          <li class="list-group-item d-flex align-items-center small" style="border: none;">
            <!-- صورة على اليسار -->
            <img :src="require('@/assets/cust.svg')" class="media-icon me-3" />
            <!-- نص بجانب الصورة -->
            <div class="d-flex flex-column">
              <!-- اسم الملف -->
              <span class="text-truncate" style="font-size: 15px;">custom.js</span>
              <!-- توقيت أسفل اسم الملف -->
              <small class="text-muted" style="font-size: 12px;">2 MB 2 Dec 2022</small>
            </div>
            <!-- حجم الملف في نهاية العنصر -->
            <small class="ms-auto text-muted" style="font-size: 12px;"></small>
          </li>
        </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
</template>
<script>
export default {
  data() {
    return {
      showDialog: false,
      dialogTitle: '',
      dialogMessage: '',
      dialogIcon: ''
    };
  },
  methods: {
    openDialog(type) {
  if (type === 'rcan1') {
    this.dialogTitle = 'Block User';
    this.dialogMessage = 'You are going to block this user. Are you sure?';
    this.dialogIcon = require('@/assets/rcan1.svg'); // استخدم require لمسار الـ block
  } else if (type === 'newdlet') {
    this.dialogTitle = 'Delete User';
    this.dialogMessage = 'once you sure to delete this conversation , you will not be able to undo this action';
    this.dialogIcon = require('@/assets/newdlet.svg'); // استخدم require لمسار الـ delete
  } else if (type === 'unlock') {
    this.dialogTitle = 'Unlock User';
    this.dialogMessage = 'you are going to unblock this user , are you sure??';
    this.dialogIcon = require('@/assets/unlock.svg'); // استخدم require لمسار الـ clip
  }
  this.showDialog = true;
},

    closeDialog() {
      this.showDialog = false;
    },
    confirmAction() {
      // تنفيذ الإجراء عند النقر على Yes
      this.closeDialog();
    }
  }
};
</script>
<style>

 body {
      font-family: Arial, sans-serif;
      background-color: #F6F7F9;
    }
/* الهيدر الأول */
.header {
  background-color: #fff;
}
.btn-icon {
  background: none;
  border: none;
  padding: 8px;
}
.user-dropdown .user {
  padding: 4px;
}
.header-2 {
  background-color: #f8f9fa;
  padding: 5px;
}
.sidebar {
  width: 220px;
  background-color: #fff;
  border-right: 1px solid #ddd;
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
  padding: 20px;
}

.custom-badge {
  background-color: #DDDBFF;

  color: #635BFF;

  padding: 5px 10px;
  border-radius: 20px;
}
.action-icon {
  margin-right: 15px;
}
.chat-messages .bg-primary {
  background-color: #007bff;
}
.chat-messages .bg-light {
  background-color: #f8f9fa;
}
.media-item img {
  width: 100px;
  height: 48px;
}

.list-group-item {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.list-group-item {
      display: flex;
      align-items: center;
      padding: 10px 15px;
      background-color: white;
      border-radius: 8px;
  
      transition: background-color 0.3s;
    }
.recent-chats {
      max-width: 400px; /* يمكنك ضبط العرض هنا ليتناسب مع التصميم */
      margin: 0 auto; /* توسيط القائمة */
    }
    .list-group-item img {
      border-radius: 50%;
      width: 48px;
      height: 48px;
      margin-right: 15px;
    }
    /* معلومات المحادثة */
    .chat-info {
      flex-grow: 1;
    }
    /* اسم الشخص */
    .chat-info h3 {
      font-size: 15px;
      margin: 0;
      color: #333;
    }

    /* نص المحادثة */
    .chat-info small {
      font-size: 12px;
      color: #888;
    }

    /* الوقت */
    .list-group-item small.text-muted {
      font-size: 12px;
      color: #888;
    }

    /* ضبط المسافات بين العناصر */
    .list-group-item + .list-group-item {
      margin-top: 10px;
    }
    .dialog-overlay {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: rgba(0, 0, 0, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 1000;
}

/* Dialog content */
.dialog-content {
  background-color: white;
  padding: 20px;
  border-radius: 10px;
  text-align: center;
  width: 320px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

/* Dialog header */
.dialog-header {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-bottom: 20px;
}

/* Dialog icon */
.dialog-icon {
  width: 40px;
  height: 40px;
  margin-bottom: 20px;
}

/* Dialog title */
.dialog-title {
  font-size: 18px;
  font-weight: 600;
  margin: 0;
  color: #333;
}

/* Dialog message */
.dialog-message {
  font-size: 14px;
  color: #666;
  margin-bottom: 20px;
}

/* Dialog actions (buttons) */
.dialog-actions {
  display: flex;
  justify-content: space-between;
}

/* Cancel button */
.btn-cancel {
  background-color: #ccc;
  color: #333;
  border: none;
  padding: 10px 20px;
  border-radius: 5px;
  cursor: pointer;
  font-size: 14px;
}

/* Confirm button */
.btn-confirm {
  background-color: #635bff;
  color: white;
  border: none;
  padding: 10px 20px;
  border-radius: 5px;
  cursor: pointer;
  font-size: 14px;
}

.btn-cancel:hover, .btn-confirm:hover {
  opacity: 0.9;
}
</style>