# Markdown Meeting Notes → Google Doc (Colab)

This repo contains a Google Colab notebook that converts markdown meeting notes into a well-formatted Google Doc using the **Google Docs API**.

## Features
- Creates a Google Doc programmatically
- Heading mapping:
  - `#` → Heading 1
  - `##` → Heading 2
  - `###` → Heading 3
- Nested bullet hierarchy with indentation
- Markdown checkboxes `- [ ]` → Google Docs checkboxes (checklist)
- Styles @mentions (bold + color)
- Styles footer lines after `---` (italic + smaller + gray)

## Dependencies
Installed in the notebook:
- `google-api-python-client`
- `google-auth-httplib2`
- `google-auth-oauthlib`

## Run in Colab
1. Open `markdown_to_gdoc_colab.ipynb` in Google Colab.
2. Run the install cell.
3. Authenticate when prompted.
4. Run the final cell and open the printed Docs URL.

## Notes / Extending
The parser is intentionally small and tailored to meeting-note markdown. For broader markdown support, extend the parser or use a markdown AST library and map nodes to Docs API requests.
