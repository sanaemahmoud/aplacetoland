A PLACE TO LAND — WEBSITE + WRITING DASHBOARD

Files to upload to the ROOT of the existing GitHub repository (sanaemahmoud/a-place-to-land):
- index.html (replace the existing one)
- admin/ (new folder containing index.html and config.yml)
- content/ (new folder; posts can be created inside it by the CMS)

After committing these files, Netlify should automatically deploy.

Dashboard URL:
https://aplacetolandsm.netlify.app/admin/

Important setup after deployment:
1. In Netlify Identity, keep registration set to Invite only.
2. In Netlify Identity, invite the owner's email address.
3. Accept the invitation from the email on the same site domain.
4. Visit /admin/ and log in.

The CMS uses Netlify Identity + Git Gateway. Netlify currently labels Git Gateway deprecated; it may continue functioning where enabled, but new configurations are not recommended. This starter is configured for the service the site owner already enabled. If Git Gateway fails, switch to a maintained GitHub OAuth/PKCE backend before relying on it.

New published essays are stored as JSON files in content/posts and are loaded into the Journal page from the public GitHub repository. Do not put private or unpublished writing into this public repository; only publish essays you intend to make public.
