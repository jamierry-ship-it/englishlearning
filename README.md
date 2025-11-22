[deepseek_html_20251122_efe011.html](https://github.com/user-attachments/files/23692277/deepseek_html_20251122_efe011.html)
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>培训流程 - 横向展示</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', 'Microsoft YaHei', sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #f0f4f8 0%, #d9e2ec 100%);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }
        
        .container {
            max-width: 1100px;
            width: 100%;
            background: white;
            border-radius: 16px;
            box-shadow: 0 8px 24px rgba(0, 0, 0, 0.08);
            padding: 30px;
        }
        
        h1 {
            text-align: center;
            color: #2d3748;
            margin-bottom: 8px;
            font-weight: 700;
            font-size: 28px;
        }
        
        .subtitle {
            text-align: center;
            color: #718096;
            margin-bottom: 30px;
            font-size: 16px;
        }
        
        .flow-container {
            display: flex;
            justify-content: space-between;
            align-items: stretch;
            margin-bottom: 20px;
        }
        
        .step {
            flex: 1;
            display: flex;
            flex-direction: column;
            align-items: center;
            margin: 0 8px;
            position: relative;
        }
        
        /* 步骤之间的连接线 */
        .step:not(:last-child)::after {
            content: '';
            position: absolute;
            top: 40px;
            right: -8px;
            width: 16px;
            height: 2px;
            background: #cbd5e0;
            z-index: 1;
        }
        
        .step-icon {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            margin-bottom: 16px;
            font-size: 32px;
            color: white;
            box-shadow: 0 6px 16px rgba(0, 0, 0, 0.12);
            z-index: 2;
            position: relative;
        }
        
        .step-1 .step-icon { background: linear-gradient(135deg, #4a6cf7, #6a93ff); }
        .step-2 .step-icon { background: linear-gradient(135deg, #ff7eb3, #ff758c); }
        .step-3 .step-icon { background: linear-gradient(135deg, #43e97b, #38f9d7); }
        .step-4 .step-icon { background: linear-gradient(135deg, #ffd166, #ffb347); }
        .step-5 .step-icon { background: linear-gradient(135deg, #9b5de5, #f15bb5); }
        
        .step-card {
            background: white;
            border-radius: 12px;
            padding: 20px 16px;
            width: 100%;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.06);
            border: 1px solid #e2e8f0;
            text-align: center;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
        }
        
        .step-title {
            font-size: 16px;
            font-weight: 700;
            margin-bottom: 12px;
            color: #2d3748;
        }
        
        .step-content {
            color: #718096;
            font-size: 13px;
            line-height: 1.5;
            flex-grow: 1;
            margin-bottom: 12px;
        }
        
        .step-content ul {
            list-style: none;
            text-align: left;
        }
        
        .step-content li {
            margin-bottom: 6px;
            position: relative;
            padding-left: 12px;
        }
        
        .step-content li::before {
            content: '•';
            position: absolute;
            left: 0;
            color: #4a6cf7;
            font-weight: bold;
        }
        
        .link-area {
            padding: 12px;
            background: #f7fafc;
            border-radius: 8px;
            border: 1px dashed #cbd5e0;
            text-align: center;
            transition: all 0.2s ease;
            cursor: pointer;
        }
        
        .link-area:hover {
            background: #edf2f7;
            border-color: #4a6cf7;
        }
        
        .link-placeholder {
            color: #4a6cf7;
            font-weight: 600;
            font-size: 14px;
        }
        
        .step-number {
            position: absolute;
            top: -8px;
            left: 50%;
            transform: translateX(-50%);
            background: #4a6cf7;
            color: white;
            width: 24px;
            height: 24px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 12px;
            font-weight: bold;
            box-shadow: 0 2px 6px rgba(74, 108, 247, 0.4);
        }
        
        .footer {
            text-align: center;
            margin-top: 20px;
            color: #718096;
            font-size: 13px;
        }
        
        /* 响应式设计 */
        @media (max-width: 900px) {
            .flow-container {
                flex-wrap: wrap;
            }
            
            .step {
                width: 48%;
                margin-bottom: 20px;
            }
            
            .step:not(:last-child)::after {
                display: none;
            }
        }
        
        @media (max-width: 576px) {
            .step {
                width: 100%;
            }
            
            .container {
                padding: 20px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>新教师培训流程</h1>
        <p class="subtitle">五个环节完成培训，快速上岗接单</p>
        
        <div class="flow-container">
            <!-- 第一阶段 -->
            <div class="step step-1">
                <div class="step-number">1</div>
                <div class="step-icon">
                    <i class="fas fa-file-signature"></i>
                </div>
                <div class="step-card">
                    <h3 class="step-title">签约入职</h3>
                    <div class="step-content">
                        <ul>
                            <li>合同签署</li>
                            <li>简历提交</li>
                        </ul>
                    </div>
                    <div class="link-area">
                        <div class="link-placeholder">【查看模板】</div>
                    </div>
                </div>
            </div>
            
            <!-- 第二阶段 -->
            <div class="step step-2">
                <div class="step-number">2</div>
                <div class="step-icon">
                    <i class="fas fa-book"></i>
                </div>
                <div class="step-card">
                    <h3 class="step-title">规章学习</h3>
                    <div class="step-content">
                        <ul>
                            <li>教师守则</li>
                            <li>工作流程</li>
                        </ul>
                    </div>
                    <div class="link-area">
                        <div class="link-placeholder">【开始学习】</div>
                    </div>
                </div>
            </div>
            
            <!-- 第三阶段 -->
            <div class="step step-3">
                <div class="step-number">3</div>
                <div class="step-icon">
                    <i class="fas fa-compass"></i>
                </div>
                <div class="step-card">
                    <h3 class="step-title">方向选择</h3>
                    <div class="step-content">
                        <ul>
                            <li>商务英语</li>
                            <li>日常口语</li>
                            <li>零基础教学</li>
                        </ul>
                    </div>
                    <div class="link-area">
                        <div class="link-placeholder">【选择方向】</div>
                    </div>
                </div>
            </div>
            
            <!-- 第四阶段 -->
            <div class="step step-4">
                <div class="step-number">4</div>
                <div class="step-icon">
                    <i class="fas fa-video"></i>
                </div>
                <div class="step-card">
                    <h3 class="step-title">磨课考核</h3>
                    <div class="step-content">
                        <ul>
                            <li>Demo录制</li>
                            <li>教学反馈</li>
                        </ul>
                    </div>
                    <div class="link-area">
                        <div class="link-placeholder">【开始磨课】</div>
                    </div>
                </div>
            </div>
            
            <!-- 第五阶段 -->
            <div class="step step-5">
                <div class="step-number">5</div>
                <div class="step-icon">
                    <i class="fas fa-briefcase"></i>
                </div>
                <div class="step-card">
                    <h3 class="step-title">上岗接单</h3>
                    <div class="step-content">
                        <ul>
                            <li>熟悉排课流程</li>
                            <li>正式授课</li>
                        </ul>
                    </div>
                    <div class="link-area">
                        <div class="link-placeholder">【进入系统】</div>
                    </div>
                </div>
            </div>
        </div>
        
        <div class="footer">
            <p>点击各环节链接区域可添加相关操作链接</p>
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // 添加链接区域点击效果
            const linkAreas = document.querySelectorAll('.link-area');
            linkAreas.forEach(area => {
                area.addEventListener('click', function() {
                    const stageTitle = this.closest('.step').querySelector('.step-title').textContent;
                    const linkText = this.querySelector('.link-placeholder').textContent;
                    alert(`为 ${stageTitle} 环节添加操作链接\n\n当前链接文本: ${linkText}\n\n您可以将此文本替换为实际链接`);
                });
            });
            
            // 添加卡片悬停效果
            const stepCards = document.querySelectorAll('.step-card');
            stepCards.forEach(card => {
                card.addEventListener('mouseenter', function() {
                    this.style.transform = 'translateY(-5px)';
                    this.style.boxShadow = '0 8px 20px rgba(0, 0, 0, 0.12)';
                });
                
                card.addEventListener('mouseleave', function() {
                    this.style.transform = 'translateY(0)';
                    this.style.boxShadow = '0 4px 12px rgba(0, 0, 0, 0.06)';
                });
            });
        });
    </script>
</body>
</html>
