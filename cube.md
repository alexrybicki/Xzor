<div class="container">
    <header>
        <a class="no-underline" href="./" >
        <h1 class='xzor-ascii-banner'>██╗&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;██╗███████╗&nbsp;&nbsp;&nbsp;██████╗&nbsp;&nbsp;&nbsp;██████╗&nbsp;&nbsp;&nbsp;<br>
             ╚██╗██╔╝╚══███╔╝██╔═══██╗██╔══██╗<br>
              &nbsp;&nbsp;&nbsp;╚███╔╝&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;███╔╝&nbsp;&nbsp;&nbsp;██║&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;██║██████╔╝<br>
            &nbsp;&nbsp;&nbsp;██╔██╗&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;███╔╝&nbsp;&nbsp;&nbsp;&nbsp;██║&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;██║██╔══██╗<br>
           ██╔╝&nbsp;&nbsp;&nbsp;██╗███████╗╚██████╔╝██║&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;██║<br>
            ╚═╝&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;╚═╝╚══════╝&nbsp;&nbsp;&nbsp;╚═════╝&nbsp;&nbsp;&nbsp;╚═╝&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;╚═╝</h1></a><br>
        <p class="subtitle">Gaming Enthusiast & Digital Warrior</p>
        <p class="tagline">Exploring the cosmos, one game at a time</p>
    </header>
<!--      <div class="profile-section">
        <h2 class="section-title centered-title alt">Filler Test Text</h2>
        <p class="about-text">
           This is just some filler testing text. Yay. 😃
        </p>
    </div> -->
  <style>
/*         body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            color: white;
        }
        .container {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 30px;
            box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
            border: 1px solid rgba(255, 255, 255, 0.18);
        }
        h1 {
            text-align: center;
            margin-bottom: 30px;
            font-size: 2.5em;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        } */
        .input-group {
            margin-bottom: 20px;
        }
        label {
            display: block;
            margin-bottom: 8px;
            font-weight: bold;
            font-size: 1.1em;
        }
        input, select {
            width: 100%;
            padding: 12px;
            border: none;
            border-radius: 10px;
            font-size: 16px;
            background: rgba(255, 255, 255, 0.2);
            background-color: #232731;
            color: white;
            backdrop-filter: blur(5px);
        }
        input::placeholder {
            color: rgba(255, 255, 255, 0.7);
        }
       button {
            background: linear-gradient(45deg, #ff6b6b, #ffa500);
            color: white;
            padding: 15px 30px;
            border: none;
            border-radius: 50px;
            font-size: 18px;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s ease;
            display: block;
            margin: 30px auto;
            box-shadow: 0 4px 15px rgba(0,0,0,0.2);
        }
        button:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.3);
        }
        button:active {
            transform: translateY(0);
        }
        .info {
            background: rgba(255, 255, 255, 0.1);
            padding: 20px;
            border-radius: 10px;
            margin: 20px 0;
            border-left: 4px solid #ffa500;
        }
        .preview {
            text-align: center;
            margin: 20px 0;
            padding: 20px;
            background: rgba(255, 255, 255, 0.05);
            border-radius: 10px;
        }
        .cube-container {
            perspective: 300px;
            margin: 20px auto;
            width: 100px;
            height: 100px;
        }
        .cube-visual {
            position: relative;
            width: 80px;
            height: 80px;
            margin: 0 auto;
            transform-style: preserve-3d;
            animation: rotateCube 8s infinite linear;
        }
        .cube-face {
            position: absolute;
            width: 80px;
            height: 80px;
            border: 2px solid rgba(255, 255, 255, 0.3);
            border-radius: 8px;
        }
        .cube-face.front {
            background: linear-gradient(45deg, #ff6b6b, #ffa500);
            transform: rotateY(0deg) translateZ(40px);
        }
        .cube-face.back {
            background: linear-gradient(45deg, #ff4757, #ff3838);
            transform: rotateY(180deg) translateZ(40px);
        }
        .cube-face.right {
            background: linear-gradient(45deg, #ffa500, #ff9f43);
            transform: rotateY(90deg) translateZ(40px);
        }
        .cube-face.left {
            background: linear-gradient(45deg, #ff3838, #ff6b6b);
            transform: rotateY(-90deg) translateZ(40px);
        }
        .cube-face.top {
            background: linear-gradient(45deg, #ff9f43, #feca57);
            transform: rotateX(90deg) translateZ(40px);
        }
        .cube-face.bottom {
            background: linear-gradient(45deg, #ff4757, #c44569);
            transform: rotateX(-90deg) translateZ(40px);
        }
        @keyframes rotateCube {
            0% { transform: rotateX(0deg) rotateY(0deg) rotateZ(0deg); }
            25% { transform: rotateX(90deg) rotateY(90deg) rotateZ(0deg); }
            50% { transform: rotateX(180deg) rotateY(180deg) rotateZ(90deg); }
            75% { transform: rotateX(270deg) rotateY(270deg) rotateZ(180deg); }
            100% { transform: rotateX(360deg) rotateY(360deg) rotateZ(270deg); }
        }
        .success-message {
            background: rgba(76, 175, 80, 0.3);
            color: white;
            padding: 15px;
            border-radius: 10px;
            margin: 20px 0;
            border-left: 4px solid #4CAF50;
            display: none;
        }
        ul {
            padding-left: 50px;
        }
    </style>
    <div class="profile-section">
        <h2 class="section-title centered-title alt">🎲 STL Cube Generator</h2>
        <div class="input-group">
            <label for="size">Cube Size:</label>
            <input type="number" id="size" value="25.4" step="0.1" min="0.1" placeholder="Enter size in mm">
        </div>
        <div class="input-group">
            <label for="unit">Unit:</label>
            <select id="unit">
                <option value="mm">Millimeters (mm)</option>
                <option value="inch" selected>Inches (will convert to mm)</option>
                <option value="cm">Centimeters (cm)</option>
            </select>
        </div>
        <div class="input-group">
            <label for="filename">Filename:</label>
            <input type="text" id="filename" value="cube_1inch.stl" placeholder="Enter filename">
        </div>
        <div class="preview">
            <h3>Preview</h3><br>
            <div class="cube-container">
                <div class="cube-visual">
                    <div class="cube-face front"></div>
                    <div class="cube-face back"></div>
                    <div class="cube-face right"></div>
                    <div class="cube-face left"></div>
                    <div class="cube-face top"></div>
                    <div class="cube-face bottom"></div>
                </div>
            </div>
            <p id="dimensions">Dimensions: 25.4mm × 25.4mm × 25.4mm</p>
        </div>
        <button onclick="generateCube()">Generate & Download STL</button>
        <div id="successMessage" class="success-message">
            ✅ STL file generated and downloaded successfully!
        </div>
    </div>
    <div class="profile-section">
        <div class="about-text">
            <h3 class="section-title centered-title alt">ℹ️ How it works:</h3>
            <div>
                <ul>
                    <li>Creates a perfect cube with the dimensions you specify</li>
                    <li>Generates a binary STL file compatible with all 3D printers</li>
                    <li>Downloads directly to your device</li>
                    <li>Uses 12 triangles to define the cube faces</li>
                    <li>File size will be approximately 684 bytes</li>
                </ul>
            </div>
        </div>
    </div>
    <script>
        function createCubeSTL(size, filename = "cube.stl") {
            // Define the 8 vertices of a cube
            const h = size / 2;
            const vertices = [
                [-h, -h, -h],  // 0: bottom-back-left
                [+h, -h, -h],  // 1: bottom-back-right
                [+h, +h, -h],  // 2: bottom-front-right
                [-h, +h, -h],  // 3: bottom-front-left
                [-h, -h, +h],  // 4: top-back-left
                [+h, -h, +h],  // 5: top-back-right
                [+h, +h, +h],  // 6: top-front-right
                [-h, +h, +h],  // 7: top-front-left
            ];
            // Define the 12 triangular faces
            const faces = [
                [0, 2, 1], [0, 3, 2],  // Bottom face
                [4, 5, 6], [4, 6, 7],  // Top face
                [3, 6, 2], [3, 7, 6],  // Front face
                [0, 1, 5], [0, 5, 4],  // Back face
                [1, 2, 6], [1, 6, 5],  // Right face
                [0, 4, 7], [0, 7, 3],  // Left face
            ];
            // Calculate normal vector for a triangle
            function calculateNormal(v0, v1, v2) {
                const edge1 = [v1[0] - v0[0], v1[1] - v0[1], v1[2] - v0[2]];
                const edge2 = [v2[0] - v0[0], v2[1] - v0[1], v2[2] - v0[2]];
                // Cross product
                const normal = [
                    edge1[1] * edge2[2] - edge1[2] * edge2[1],
                    edge1[2] * edge2[0] - edge1[0] * edge2[2],
                    edge1[0] * edge2[1] - edge1[1] * edge2[0]
                ];
                // Normalize
                const length = Math.sqrt(normal[0] * normal[0] + normal[1] * normal[1] + normal[2] * normal[2]);
                if (length > 0) {
                    normal[0] /= length;
                    normal[1] /= length;
                    normal[2] /= length;
                }
                return normal;
            }
            // Helper functions for binary data
            function floatToBytes(value) {
                const buffer = new ArrayBuffer(4);
                const view = new DataView(buffer);
                view.setFloat32(0, value, true);
                return new Uint8Array(buffer);
            }
            function uint32ToBytes(value) {
                const buffer = new ArrayBuffer(4);
                const view = new DataView(buffer);
                view.setUint32(0, value, true);
                return new Uint8Array(buffer);
            }
            function uint16ToBytes(value) {
                const buffer = new ArrayBuffer(2);
                const view = new DataView(buffer);
                view.setUint16(0, value, true);
                return new Uint8Array(buffer);
            }
            // Build STL data
            const data = [];
            // 80-byte header
            const headerText = 'Generated cube for 3D printing - Browser STL Generator';
            const header = new Uint8Array(80);
            for (let i = 0; i < Math.min(headerText.length, 80); i++) {
                header[i] = headerText.charCodeAt(i);
            }
            data.push(header);
            // Triangle count
            data.push(uint32ToBytes(faces.length));
            // Write each triangle
            faces.forEach(face => {
                const v0 = vertices[face[0]];
                const v1 = vertices[face[1]];
                const v2 = vertices[face[2]];
                const normal = calculateNormal(v0, v1, v2);
                // Normal vector
                data.push(floatToBytes(normal[0]));
                data.push(floatToBytes(normal[1]));
                data.push(floatToBytes(normal[2]));
                // Vertices
                [v0, v1, v2].forEach(vertex => {
                    data.push(floatToBytes(vertex[0]));
                    data.push(floatToBytes(vertex[1]));
                    data.push(floatToBytes(vertex[2]));
                });                
                // Attribute byte count
                data.push(uint16ToBytes(0));
            });            
            // Combine all data
            const totalLength = data.reduce((sum, chunk) => sum + chunk.length, 0);
            const binaryData = new Uint8Array(totalLength);
            let offset = 0;            
            data.forEach(chunk => {
                binaryData.set(chunk, offset);
                offset += chunk.length;
            });            
            return binaryData;
        }        
        function downloadFile(data, filename) {
            const blob = new Blob([data], { type: 'application/octet-stream' });
            const url = URL.createObjectURL(blob);            
            const a = document.createElement('a');
            a.href = url;
            a.download = filename;
            document.body.appendChild(a);
            a.click();
            document.body.removeChild(a);
            URL.revokeObjectURL(url);
        }        
        function updatePreview() {
            const sizeInput = document.getElementById('size');
            const unitSelect = document.getElementById('unit');
            const dimensionsEl = document.getElementById('dimensions');            
            let size = parseFloat(sizeInput.value) || 25.4;
            const unit = unitSelect.value;            
            // Convert to mm for internal calculations
            let sizeInMM = size;
            if (unit === 'inch') {
                sizeInMM = size * 25.4;
            } else if (unit === 'cm') {
                sizeInMM = size * 10;
            }
            dimensionsEl.textContent = `Dimensions: ${sizeInMM.toFixed(1)}mm × ${sizeInMM.toFixed(1)}mm × ${sizeInMM.toFixed(1)}mm`;
        }
        function generateCube() {
            const sizeInput = document.getElementById('size');
            const unitSelect = document.getElementById('unit');
            const filenameInput = document.getElementById('filename');
            const successMessage = document.getElementById('successMessage');            
            let size = parseFloat(sizeInput.value) || 1;
            const unit = unitSelect.value;
            const filename = filenameInput.value || 'cube.stl';            
            // Convert to mm
            let sizeInMM = size;
            if (unit === 'inch') {
                sizeInMM = size * 25.4;
            } else if (unit === 'cm') {
                sizeInMM = size * 10;
            }            
            try {
                const stlData = createCubeSTL(sizeInMM, filename);
                downloadFile(stlData, filename);                
                successMessage.style.display = 'block';
                setTimeout(() => {
                    successMessage.style.display = 'none';
                }, 3000);                
                console.log(`Generated ${filename}: ${sizeInMM.toFixed(1)}mm cube with ${stlData.length} bytes`);
            } catch (error) {
                alert('Error generating STL file: ' + error.message);
                console.error(error);
            }
        }        
        // Update preview when inputs change
        document.getElementById('size').addEventListener('input', updatePreview);
        document.getElementById('unit').addEventListener('change', function() {
            const sizeInput = document.getElementById('size');
            const unit = this.value;            
            // Auto-adjust default values based on unit
            if (unit === 'inch') {
                sizeInput.value = '1.0';
            } else if (unit === 'mm') {
                sizeInput.value = '25.4';
            } else if (unit === 'cm') {
                sizeInput.value = '2.54';
            }
            updatePreview();
        });        
        // Initialize
        updatePreview();
    </script>
    
