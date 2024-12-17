
# Simple Calculator

โปรแกรมนี้เป็นเครื่องคิดเลขพื้นฐานที่ใช้สำหรับการคำนวณทางคณิตศาสตร์ เช่น การบวก, การลบ, การคูณ, การหาร และสามารถล้างข้อมูลได้  
เขียนขึ้นโดย **Tanapattara Wongkhamchan**  
รหัสนักศึกษา: 670000000-0  
หลักสูตร: **Computer and Information Science**, KKU  

---

## ฟังก์ชันที่รองรับ  
โปรแกรมรองรับการทำงาน 5 ฟังก์ชันหลักดังนี้:  
1. **ปุ่มบวก (+)** : ใช้สำหรับคำนวณผลรวมของสองจำนวน  
2. **ปุ่มลบ (-)** : ใช้สำหรับหาค่าผลต่างระหว่างสองจำนวน  
3. **ปุ่มคูณ (*)** : ใช้สำหรับหาผลคูณของสองจำนวน  
4. **ปุ่มหาร (/)** : ใช้สำหรับหาค่าผลหารของสองจำนวน พร้อมตรวจสอบกรณีหารด้วยศูนย์  
5. **ปุ่มล้างข้อมูล** : ใช้สำหรับล้างข้อมูลทั้งหมดในช่องป้อนเลขและผลลัพธ์  

---

## วิธีการใช้งานโปรแกรม  

1. **การป้อนข้อมูล**  
   - ป้อนค่าตัวเลขที่ช่อง `Number 1` และ `Number 2`  

2. **การคำนวณ**  
   - เลือกปุ่มที่ต้องการ:  
     - ปุ่ม `+` : ทำการบวกเลข  
     - ปุ่ม `-` : ทำการลบเลข  
     - ปุ่ม `*` : ทำการคูณเลข  
     - ปุ่ม `/` : ทำการหารเลข  
   - ผลลัพธ์จะแสดงที่ช่อง `Result`  

3. **การลบข้อมูล**  
   - กดปุ่ม **Clear** เพื่อล้างข้อมูลทั้งหมด  

---

## ตัวอย่างการทำงาน  

### 1. การบวกเลข  
- **Input**:  
   - Number 1: `10`  
   - Number 2: `5`  
- **Output**:  
   - Result: `15`  

### 2. การลบเลข  
- **Input**:  
   - Number 1: `20`  
   - Number 2: `8`  
- **Output**:  
   - Result: `12`  

### 3. การคูณเลข  
- **Input**:  
   - Number 1: `3`  
   - Number 2: `4`  
- **Output**:  
   - Result: `12`  

### 4. การหารเลข  
- **Input**:  
   - Number 1: `10`  
   - Number 2: `2`  
- **Output**:  
   - Result: `5`  

### 5. กรณีหารด้วยศูนย์  
- **Input**:  
   - Number 1: `10`  
   - Number 2: `0`  
- **Output**:  
   - Result: `หารด้วย 0 ไม่ได้`  

---

## คำอธิบายโค้ด  
- **`Int32.Parse()`** : ใช้แปลงข้อความ (string) ที่ผู้ใช้งานป้อน เป็นตัวเลขจำนวนเต็ม (integer)  
- **`try-catch`** : ใช้สำหรับจัดการข้อผิดพลาด เช่น ผู้ใช้งานป้อนข้อความที่ไม่ใช่ตัวเลข  
- **ตรวจสอบหารด้วยศูนย์** : ใช้คำสั่ง `if` เพื่อตรวจสอบก่อนทำการหาร  

ตัวอย่างโค้ดสำหรับปุ่มบวก:  
```csharp
private void buttonAdd_Click(object sender, EventArgs e)
{
    int num1 = Int32.Parse(txtNum1.Text);
    int num2 = Int32.Parse(txtNum2.Text);
    int result = num1 + num2;
    txtResult.Text = result.ToString();
}
```

---

## เครื่องมือที่ใช้  
- **Visual Studio** สำหรับการพัฒนาโปรแกรม  
- ภาษาโปรแกรม: **C#** (Windows Forms Application)  

---

## การปรับปรุงเพิ่มเติม  
1. เพิ่มการแสดงประวัติการคำนวณ  
2. ปรับแต่ง UI ให้ดูสวยงามมากขึ้น  
3. รองรับการคำนวณทศนิยมในทุกฟังก์ชัน  

---

## ผู้จัดทำ  
**Tanapattara Wongkhamchan**  
รหัสนักศึกษา: 670000000-0  
**Computer and Information Science**, KKU  
