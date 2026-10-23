# Liquid Glass Style

Use this reference when the user requests liquid glass or the material clearly serves the project concept. Treat iOS 26 Liquid Glass as an aesthetic reference for non-native work, not a default theme or a claim of native iOS behavior.

## Visual direction

Build a translucent, luminous glass material with fluid sculptural curves, clear depth layers, soft diffused light, detailed caustics, complex reflections, bright highlights, ambient occlusion, and cinematic volumetric light. Use a quiet neutral background when the composition allows it. Keep the subject and silhouette specific to the project.

### Copy-ready image prompt

**English**

> Ultra-detailed, photorealistic 3D liquid-glass rendering with a futuristic, translucent, luminous Liquid Glass aesthetic inspired by iOS 26. Sculptural fluid curves, soft diffused lighting, detailed caustics, and complex reflections. [Describe the project-specific subject, silhouette, colors, and composition.] Float it over a minimal neutral background, with soft liquid edges, clear depth layers, crisp highlights, realistic ambient occlusion, a refined luxury finish, cinematic focus, and volumetric light passing through the glass. Octane-like rendering, photoreal finish.

**Español**

> Render 3D hiperrealista y ultra detallado de vidrio líquido futurista, translúcido y brillante, inspirado en la estética Liquid Glass de iOS 26. Curvas fluidas y escultóricas, iluminación suave y difusa, cáusticas detalladas y reflejos complejos. [Describe el objeto, la silueta, los colores y la composición propios del proyecto.] Flota sobre un fondo neutro y minimalista, con bordes líquidos suaves, capas de profundidad claras, reflejos intensos, oclusión ambiental realista, acabado de lujo, enfoque cinematográfico y luz volumétrica atravesando el vidrio. Renderizado con acabado tipo Octane y resultado fotorealista.

Replace the bracketed direction with the real asset or interface element. Preserve its recognizable silhouette, project palette, purpose, and required background or transparency. Avoid arbitrary lettering, logos, extra objects, or effects unless requested. For small logos and icons, simplify internal detail so the silhouette remains recognizable at small sizes.

## Apply it by surface

- **Image or brand asset:** use the prompt above as a material and lighting recipe. Request a transparent background only when the output needs one; otherwise use a clean background that fits the brand.
- **Web interface:** reserve glass for a few meaningful surfaces, such as navigation, a floating control, or a focused card. Keep text and dense data on stable, sufficiently opaque surfaces. Check contrast over the actual background, focus and pressed states, and a solid fallback when backdrop blur is unavailable.
- **Native iOS 26 interface:** use the host's current platform documentation and native glass components. If available, consult ecc:liquid-glass-design for implementation details. Do not apply native iOS APIs to web code.
- **Motion:** use brief motion only to show depth, state, or spatial continuity. Respect reduced-motion preferences and keep static content clear.

## Craft limits

Use blur, transparency, layered reflections, and large glass surfaces sparingly. Avoid stacking many blurred layers or animating broad, full-screen glass effects; both can obscure content and increase rendering cost. Recheck the result on light and dark backgrounds, at small and narrow sizes, and with keyboard focus. Keep essential text readable without relying on reflections or background blur.