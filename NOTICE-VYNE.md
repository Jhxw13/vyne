# VYNE: origem, licença e estado do rebrand

## Origem
VYNE Video Editor é um **fork do Concat** (https://github.com/jub0t/Concat), copyright 2026 Jareer e contribuidores do Concat. O VYNE não é oficial, nem mantido ou endossado pelo projeto Concat.

## Licença
O código herdado é AGPL-3.0-or-later. Versões distribuídas do VYNE devem manter essa licença, os avisos de copyright originais (cabeçalhos SPDX nos arquivos) e oferecer o código-fonte aos usuários, inclusive quando o app for usado por rede (AGPL §13). O nome e o logo do Concat não estão licenciados (ver `TRADEMARK.md` do upstream, preservado em `docs/UPSTREAM-README-concat.md` e no próprio arquivo). Isto não é aconselhamento jurídico.

## Já alterado
- Nome da janela e textos da interface em todos os idiomas (`locales/*.json`), exceto "Concat's mirror" (servidor de modelos do projeto original).
- Paleta: laranja VYNE como acento padrão (slot 0), playhead laranja, fundo `#0E0E0F` e painéis `#1F1F22` (tema escuro); laranja `#D46B00` no tema claro.
- Ícones do app (`assets/icons/*`, `concat.ico`) e logos SVG em `assets/vyne/`.
- Atualizador embutido desativado (`VYNE_UPDATES_ENABLED = false` em `concat-host/src/updates.rs`), pois apontava para os releases do Concat e instalaria Concat por cima do VYNE.
- README substituído (o original está em `docs/UPSTREAM-README-concat.md`).

## Ainda cita Concat (pendente)
- Instaladores: `assets/windows/concat.iss` e `concat.wxs`, `assets/linux/nfpm.yaml`, PKGBUILD, ids de app (`app.concat.editor`), `flake.nix`, CI em `.github/`.
- Logos/capturas antigos do Concat em `assets/` (concat-mark*, new_concat_logo*, editor*.png, patrocinador) e `docs/README.*.md`; scripts em `scripts/` ainda os referenciam.
- Nomes internos de crates/binário (`concat`, `concat-*`), formato de projeto `concat.json`, variável `CONCAT_LOG`, pasta de dados do usuário, textos de "Sobre"/CODE_SIGNING/CONTRIBUTING.
- Links de issues em comentários do código (inofensivos).
