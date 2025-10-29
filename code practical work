<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BLOOM COLLEGE - Student Registration Form</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.2/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body { background-color: #f8f9fa; padding: 20px; }
        .container { max-width: 800px; background: white; padding: 30px; border-radius: 8px; box-shadow: 0 2px 4px rgba(0,0,0,0.1); }
        .form-title { text-align: center; margin-bottom: 10px; font-weight: bold; }
        .form-subtitle { text-align: center; margin-bottom: 30px; font-size: 14px; }
        .section-title { font-weight: bold; margin-top: 20px; margin-bottom: 15px; text-align: center; }
    </style>
</head>
<body>
    <div class="container">
        <h4 class="form-title">BLOOM COLLEGE</h4>
        <p class="form-subtitle">Student Registration Form</p>

        <form id="regForm">
            <div class="row mb-3">
                <label class="col-sm-3 col-form-label">Student Name:</label>
                <div class="col-sm-9"><input type="text" class="form-control" id="studentName" placeholder="Ex: Juan Dela Cruz"></div>
            </div>

            <div class="row mb-3">
                <label class="col-sm-3 col-form-label">Father's Name:</label>
                <div class="col-sm-9"><input type="text" class="form-control" id="fatherName" placeholder="Ex: Juan S. Dela Cruz"></div>
            </div>

            <div class="row mb-3">
                <label class="col-sm-3 col-form-label">Mother's Name:</label>
                <div class="col-sm-9"><input type="text" class="form-control" id="motherName" placeholder="Ex: Ana P. Dela Cruz"></div>
            </div>

            <div class="row mb-3">
                <label class="col-sm-3 col-form-label">Gender:</label>
                <div class="col-sm-9">
                    <input type="radio" name="gender" value="Male"> Male
                    <input type="radio" name="gender" value="Female" class="ms-3"> Female
                </div>
            </div>

            <div class="row mb-3">
                <label class="col-sm-3 col-form-label">Date of Birth:</label>
                <div class="col-sm-9">
                    <select class="form-select">
                        <option>1st / Jan / 1972</option>
                        <option>2nd / Feb / 1973</option>
                    </select>
                </div>
            </div>

            <div class="row mb-3">
                <label class="col-sm-3 col-form-label">E-Mail:</label>
                <div class="col-sm-9"><input type="email" class="form-control" id="email"></div>
            </div>

            <div class="row mb-3">
                <label class="col-sm-3 col-form-label">Level:</label>
                <div class="col-sm-9">
                    <select class="form-select">
                        <option>First</option>
                        <option>Second</option>
                    </select>
                </div>
            </div>

            <div class="row mb-3">
                <label class="col-sm-3 col-form-label">Department:</label>
                <div class="col-sm-9">
                    <select class="form-select">
                        <option>Computer Engineering</option>
                        <option>Electrical Engineering</option>
                    </select>
                </div>
            </div>

            <div class="row mb-3">
                <label class="col-sm-3 col-form-label">To MobileN:</label>
                <div class="col-sm-9"><input type="tel" class="form-control" placeholder="Ex: 1 123 1233"></div>
            </div>

            <h5 class="section-title">Address</h5>

            <div class="row mb-3">
                <label class="col-sm-3 col-form-label">Street:</label>
                <div class="col-sm-9"><input type="text" class="form-control"></div>
            </div>

            <div class="row mb-3">
                <label class="col-sm-3 col-form-label">City:</label>
                <div class="col-sm-9"><input type="text" class="form-control"></div>
            </div>

            <div class="row mb-3">
                <label class="col-sm-3 col-form-label">Postcode:</label>
                <div class="col-sm-9"><input type="text" class="form-control"></div>
            </div>

            <div class="text-center mt-4">
                <button type="submit" class="btn btn-secondary">Register</button>
                <button type="reset" class="btn btn-secondary ms-2">Reset</button>
            </div>
        </form>
    </div>

    <!-- Modal -->
    <div class="modal fade" id="successModal" tabindex="-1">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title">Registration Successful</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
                </div>
                <div class="modal-body">Your details have been saved!</div>
                <div class="modal-footer">
                    <button type="button" class="btn btn-primary" data-bs-dismiss="modal">OK</button>
                </div>
            </div>
        </div>
    </div>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.2/js/bootstrap.bundle.min.js"></script>
    <script>
        // i. onBlur
        ['studentName', 'fatherName', 'motherName'].forEach(id => { 
            document.getElementById(id).onblur = () => console.log(id + ' field lost focus');
        }); 

        // ii. onFocus for email
        document.getElementById('email').onfocus = function() { this.style.backgroundColor = '#fffacd'; }; 
        document.getElementById('email').onblur = function() { this.style.backgroundColor = ''; };

        // iii. onChange to caps
        ['studentName', 'fatherName', 'motherName'].forEach(id => { -
            document.getElementById(id).onchange = function() { this.value = this.value.toUpperCase(); };
        }); 

        // iv. Submit with modal
        document.getElementById('regForm').onsubmit = function(e) {
            e.preventDefault();
            new bootstrap.Modal(document.getElementById('successModal')).show();
        };
    </script>
</body>
</html>
