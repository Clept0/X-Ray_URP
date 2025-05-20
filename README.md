# 🔍 X-Ray for Unity URP

<img width="902" alt="xrayTitle" src="https://github.com/user-attachments/assets/eb730c17-d420-4058-83f7-1930ff4e27c7" />

A simple X-Ray effect for Unity's Universal Render Pipeline (URP) that makes selected objects visible through obstacles. Ideal for third-person games, strategy views, and target highlighting.

---

## ⚙️ Renderer Setup

<img width="800" alt="Renderer Settings" src="https://github.com/user-attachments/assets/8ae38f4b-2ddd-4a27-9b2a-dd3110ab3b4c" />

	•	Make sure the Experimental Render Objects feature is properly configured in your URP Renderer asset.
	•	Assign a dedicated Layer (e.g., XRay, RenderAbove) to the objects that should be rendered above all others.
- Use the included **`LayerSwitchScript`** to toggle the X-Ray effect at runtime.

---

## 🎨 X-Ray Material

- The **X-Ray material** is fully customizable via Shader Graph.
- If no custom material is assigned, the object’s **original material** will be restored when X-Ray is disabled.
- Material switching is handled automatically during runtime.

---

## 🎮 Demo Scene

<img width="800" alt="Demo Scene" src="https://github.com/user-attachments/assets/7c371764-8187-4835-a6d7-cc52ef6567c3" />

---

## ✅ Features

- Compatible with Unity URP (Universal Render Pipeline)
- Easy integration and setup
- Runtime toggling via script
- Supports fallback to original materials
- Includes a working demo scene

---

## 📝 Technical Notes

This system is based on a **URP Forward Renderer Feature** called **Render Objects**, which allows specific objects to be rendered on top of others regardless of depth. The core functionality relies on this feature to achieve the "see-through" or X-Ray effect.

The included **Shader Graph-based material** is purely **optional** and only affects visual style (e.g., transparency, glow, dissolve effects).  

You can use:

- Your own X-Ray styled material,
- The default material of the object,
- Or no material override at all.

This makes the system flexible: it works even without a custom shader – the **Render Feature handles the actual visibility**.

- Tested with **Unity 2022.3.12f1 LTS** and **URP**
- Shader Graph-based – **not compatible with Built-in Render Pipeline**

---

## 🧠 Credits

Based on this [YouTube tutorial](https://www.youtube.com/watch?v=WmnYhIwWYfU&t=193s) by Binary Lunar
